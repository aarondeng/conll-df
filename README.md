# CONLL-U to Pandas DataFrame

Turn [CONLL-U documents](http://universaldependencies.org/format.html) into [Pandas DataFrames](http://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.html) for easy NLP!

## Install

```shell
pip install conll-df
```

## Usage

```shell
curl -O https://github.com/UniversalDependencies/UD_English/raw/master/en-ud-train.conllu
```

```python
from conll_df import conll_df
path = 'en-ud-train.txt.conllu'
df = conll_df(path, file_index=False)
df.head(40).to_html()
```

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th></th>
      <th>w</th>
      <th>l</th>
      <th>x</th>
      <th>p</th>
      <th>g</th>
      <th>f</th>
      <th>e</th>
      <th>type</th>
      <th>gender</th>
      <th>Case</th>
      <th>Definite</th>
      <th>Degree</th>
      <th>Foreign</th>
      <th>Gender</th>
      <th>Mood</th>
      <th>Number</th>
      <th>Person</th>
      <th>Poss</th>
      <th>Reflex</th>
      <th>Tense</th>
      <th>Voice</th>
      <th>Type</th>
    </tr>
    <tr>
      <th>s</th>
      <th>i</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th rowspan="10" valign="top">1</th>
      <th>1.0</th>
      <td>Al</td>
      <td>Al</td>
      <td>PROPN</td>
      <td>NNP</td>
      <td>0</td>
      <td>root</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Sing</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>2.0</th>
      <td>-</td>
      <td>-</td>
      <td>PUNCT</td>
      <td>HYPH</td>
      <td>1</td>
      <td>punct</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>3.0</th>
      <td>Zaman</td>
      <td>Zaman</td>
      <td>PROPN</td>
      <td>NNP</td>
      <td>1</td>
      <td>flat</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Sing</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>4.0</th>
      <td>:</td>
      <td>:</td>
      <td>PUNCT</td>
      <td>:</td>
      <td>1</td>
      <td>punct</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>5.0</th>
      <td>American</td>
      <td>american</td>
      <td>ADJ</td>
      <td>JJ</td>
      <td>6</td>
      <td>amod</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Pos</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>6.0</th>
      <td>forces</td>
      <td>force</td>
      <td>NOUN</td>
      <td>NNS</td>
      <td>7</td>
      <td>nsubj</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Plur</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>7.0</th>
      <td>killed</td>
      <td>kill</td>
      <td>VERB</td>
      <td>VBD</td>
      <td>1</td>
      <td>parataxis</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Ind</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Past</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>8.0</th>
      <td>Shaikh</td>
      <td>Shaikh</td>
      <td>PROPN</td>
      <td>NNP</td>
      <td>7</td>
      <td>obj</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Sing</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>9.0</th>
      <td>Abdullah</td>
      <td>Abdullah</td>
      <td>PROPN</td>
      <td>NNP</td>
      <td>8</td>
      <td>flat</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Sing</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>10.0</th>
      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

      <td>...</td>

    </tr>
    <tr>
      <th rowspan="10" valign="top">2</th>
      <th>1.0</th>
      <td>[</td>
      <td>[</td>
      <td>PUNCT</td>
      <td>-LRB-</td>
      <td>10</td>
      <td>punct</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>2.0</th>
      <td>This</td>
      <td>this</td>
      <td>DET</td>
      <td>DT</td>
      <td>3</td>
      <td>det</td>
      <td>_</td>
      <td>Dem</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Sing</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Dem</td>
    </tr>
    <tr>
      <th>3.0</th>
      <td>killing</td>
      <td>killing</td>
      <td>NOUN</td>
      <td>NN</td>
      <td>10</td>
      <td>nsubj</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Sing</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>4.0</th>
      <td>of</td>
      <td>of</td>
      <td>ADP</td>
      <td>IN</td>
      <td>7</td>
      <td>case</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>5.0</th>
      <td>a</td>
      <td>a</td>
      <td>DET</td>
      <td>DT</td>
      <td>7</td>
      <td>det</td>
      <td>_</td>
      <td>Art</td>
      <td>_</td>
      <td>_</td>
      <td>Ind</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Art</td>
    </tr>
    <tr>
      <th>6.0</th>
      <td>respected</td>
      <td>respected</td>
      <td>ADJ</td>
      <td>JJ</td>
      <td>7</td>
      <td>amod</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Pos</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>7.0</th>
      <td>cleric</td>
      <td>cleric</td>
      <td>NOUN</td>
      <td>NN</td>
      <td>3</td>
      <td>nmod</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Sing</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>8.0</th>
      <td>will</td>
      <td>will</td>
      <td>AUX</td>
      <td>MD</td>
      <td>10</td>
      <td>aux</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>9.0</th>
      <td>be</td>
      <td>be</td>
      <td>AUX</td>
      <td>VB</td>
      <td>10</td>
      <td>aux</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
    </tr>
    <tr>
      <th>10.0</th>
      <td>causing</td>
      <td>cause</td>
      <td>VERB</td>
      <td>VBG</td>
      <td>0</td>
      <td>root</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>

      <td>_</td>
    </tr>
  </tbody>
</table>

## Function arguments

| Name  | Type  | Description  |
|---|---|---|
| `path`  | `str`  | Path to CONLL-U file  |
| `add_gov`  | `bool`  | Create extra columns for governor word, lemma, POS and function  |
| `skip_morph`  | `bool`  | Enable if you'd like to skip the parsing of morphological and extra fields  |
| `v2`  | `bool`/`'auto'`  | CONLL-U version of file. By default, detect from data |
| `drop` | `list` | list of column names you don't need |
| `add_meta` | `bool` | add columns for sentence-level metadata |
| `categories` | `bool` | Convert columns to categorical format where possible |
| `file_index` | `bool` | Include filename in index levels |
| `extra_fields` | `list`/`'auto'` | `Names of extra fields in the last column. By default, detect from data |
| `kwargs`  | `dict` | additional arguments to pass to `pandas.read_csv()` |

Configuring these arguments can increase speed a lot, so if speed is important to you, turn off the features you don't need.

## Where to from here?

If you're working with Python and CONLL-U, you might want to take a look at [tücan](https://github.com/interrogator/tucan), which provides a command-line and web-app interface for exploring CONLL-U datasets.

Alternatively, there's plenty of cool stuff you can do with Pandas by itself. Here are some toy examples:

### Pivot table

```python
# add a dummy 'count' of 1 to each entry
df['count'] = [1 for i in range(len(df))]
piv = df.pivot_table(values='count', columns='f', index=['x'], aggfunc=sum)
piv.fillna(0).astype(int).to_html()
```

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th>f</th>
      <th>_</th>
      <th>acl</th>
      <th>acl:relcl</th>
      <th>advcl</th>
      <th>advmod</th>
      <th>amod</th>
      <th>appos</th>
      <th>aux</th>
      <th>aux:pass</th>
      <th>case</th>
      <th>cc</th>
      <th>cc:preconj</th>
      <th>ccomp</th>
      <th>compound</th>
      <th>compound:prt</th>
      <th>conj</th>
      <th>cop</th>
      <th>csubj</th>
      <th>csubj:pass</th>
      <th>dep</th>
      <th>det</th>
      <th>det:predet</th>
      <th>discourse</th>
      <th>dislocated</th>
      <th>expl</th>
      <th>fixed</th>
      <th>flat</th>
      <th>flat:foreign</th>
      <th>goeswith</th>
      <th>iobj</th>
      <th>list</th>
      <th>mark</th>
      <th>nmod</th>
      <th>nmod:npmod</th>
      <th>nmod:poss</th>
      <th>nmod:tmod</th>
      <th>nsubj</th>
      <th>nsubj:pass</th>
      <th>nummod</th>
      <th>obj</th>
      <th>obl</th>
      <th>obl:npmod</th>
      <th>obl:tmod</th>
      <th>orphan</th>
      <th>parataxis</th>
      <th>punct</th>
      <th>reparandum</th>
      <th>root</th>
      <th>vocative</th>
      <th>xcomp</th>
    </tr>
    <tr>
      <th>x</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>ADJ</th>
      <td>1</td>
      <td>26</td>
      <td>120</td>
      <td>240</td>
      <td>100</td>
      <td>8344</td>
      <td>38</td>
      <td>0</td>
      <td>0</td>
      <td>34</td>
      <td>0</td>
      <td>0</td>
      <td>282</td>
      <td>19</td>
      <td>2</td>
      <td>842</td>
      <td>0</td>
      <td>9</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>15</td>
      <td>9</td>
      <td>63</td>
      <td>5</td>
      <td>1</td>
      <td>0</td>
      <td>88</td>
      <td>9</td>
      <td>5</td>
      <td>142</td>
      <td>124</td>
      <td>28</td>
      <td>4</td>
      <td>2</td>
      <td>167</td>
      <td>0</td>
      <td>0</td>
      <td>1239</td>
      <td>0</td>
      <td>512</td>
    </tr>
    <tr>
      <th>ADP</th>
      <td>0</td>
      <td>2</td>
      <td>11</td>
      <td>0</td>
      <td>26</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>16267</td>
      <td>2</td>
      <td>0</td>
      <td>1</td>
      <td>20</td>
      <td>732</td>
      <td>8</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>1</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>262</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>91</td>
      <td>25</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>184</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
    </tr>
    <tr>
      <th>ADV</th>
      <td>0</td>
      <td>8</td>
      <td>16</td>
      <td>60</td>
      <td>9138</td>
      <td>6</td>
      <td>0</td>
      <td>4</td>
      <td>0</td>
      <td>97</td>
      <td>60</td>
      <td>19</td>
      <td>33</td>
      <td>19</td>
      <td>12</td>
      <td>121</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>9</td>
      <td>0</td>
      <td>5</td>
      <td>131</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>380</td>
      <td>61</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>5</td>
      <td>0</td>
      <td>5</td>
      <td>12</td>
      <td>100</td>
      <td>4</td>
      <td>2</td>
      <td>4</td>
      <td>22</td>
      <td>0</td>
      <td>0</td>
      <td>190</td>
      <td>0</td>
      <td>20</td>
    </tr>
    <tr>
      <th>AUX</th>
      <td>0</td>
      <td>0</td>
      <td>15</td>
      <td>31</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>6481</td>
      <td>1325</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>8</td>
      <td>1</td>
      <td>0</td>
      <td>10</td>
      <td>4451</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>4</td>
      <td>0</td>
      <td>1</td>
      <td>13</td>
      <td>0</td>
      <td>1</td>
    </tr>
    <tr>
      <th>CCONJ</th>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>5</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>6599</td>
      <td>82</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>5</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>8</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <th>DET</th>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>10</td>
      <td>0</td>
      <td>4</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>2</td>
      <td>2</td>
      <td>5</td>
      <td>0</td>
      <td>32</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>15736</td>
      <td>162</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>22</td>
      <td>24</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>96</td>
      <td>9</td>
      <td>5</td>
      <td>76</td>
      <td>52</td>
      <td>3</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>10</td>
      <td>22</td>
      <td>2</td>
      <td>3</td>
    </tr>
    <tr>
      <th>INTJ</th>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>4</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>6</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>587</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>81</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <th>NOUN</th>
      <td>0</td>
      <td>16</td>
      <td>86</td>
      <td>181</td>
      <td>23</td>
      <td>17</td>
      <td>709</td>
      <td>0</td>
      <td>0</td>
      <td>5</td>
      <td>2</td>
      <td>0</td>
      <td>247</td>
      <td>4605</td>
      <td>0</td>
      <td>2416</td>
      <td>0</td>
      <td>3</td>
      <td>1</td>
      <td>3</td>
      <td>0</td>
      <td>0</td>
      <td>14</td>
      <td>2</td>
      <td>0</td>
      <td>24</td>
      <td>54</td>
      <td>0</td>
      <td>4</td>
      <td>37</td>
      <td>203</td>
      <td>0</td>
      <td>4602</td>
      <td>80</td>
      <td>219</td>
      <td>205</td>
      <td>4082</td>
      <td>568</td>
      <td>36</td>
      <td>6911</td>
      <td>6235</td>
      <td>359</td>
      <td>483</td>
      <td>12</td>
      <td>245</td>
      <td>12</td>
      <td>1</td>
      <td>1896</td>
      <td>22</td>
      <td>161</td>
    </tr>
    <tr>
      <th>NUM</th>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>7</td>
      <td>9</td>
      <td>15</td>
      <td>156</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>7</td>
      <td>225</td>
      <td>0</td>
      <td>74</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>50</td>
      <td>0</td>
      <td>242</td>
      <td>5</td>
      <td>1</td>
      <td>46</td>
      <td>83</td>
      <td>4</td>
      <td>2375</td>
      <td>81</td>
      <td>199</td>
      <td>7</td>
      <td>11</td>
      <td>0</td>
      <td>14</td>
      <td>0</td>
      <td>2</td>
      <td>370</td>
      <td>1</td>
      <td>7</td>
    </tr>
    <tr>
      <th>PART</th>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>9</td>
      <td>1572</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>684</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>2</td>
      <td>0</td>
      <td>17</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>7</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>3260</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>1</td>
      <td>2</td>
      <td>0</td>
      <td>9</td>
    </tr>
    <tr>
      <th>PRON</th>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>20</td>
      <td>1</td>
      <td>0</td>
      <td>11</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>21</td>
      <td>5</td>
      <td>0</td>
      <td>148</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>8</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>580</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>314</td>
      <td>1</td>
      <td>0</td>
      <td>311</td>
      <td>27</td>
      <td>3054</td>
      <td>0</td>
      <td>10348</td>
      <td>454</td>
      <td>0</td>
      <td>2362</td>
      <td>782</td>
      <td>16</td>
      <td>0</td>
      <td>0</td>
      <td>15</td>
      <td>0</td>
      <td>4</td>
      <td>80</td>
      <td>3</td>
      <td>5</td>
    </tr>
    <tr>
      <th>PROPN</th>
      <td>0</td>
      <td>3</td>
      <td>8</td>
      <td>28</td>
      <td>0</td>
      <td>12</td>
      <td>511</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>23</td>
      <td>3163</td>
      <td>0</td>
      <td>795</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1382</td>
      <td>0</td>
      <td>0</td>
      <td>22</td>
      <td>117</td>
      <td>0</td>
      <td>1545</td>
      <td>22</td>
      <td>396</td>
      <td>36</td>
      <td>1548</td>
      <td>97</td>
      <td>0</td>
      <td>527</td>
      <td>1410</td>
      <td>24</td>
      <td>50</td>
      <td>0</td>
      <td>51</td>
      <td>0</td>
      <td>1</td>
      <td>1029</td>
      <td>94</td>
      <td>45</td>
    </tr>
    <tr>
      <th>PUNCT</th>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>5</td>
      <td>100</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>23524</td>
      <td>0</td>
      <td>41</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <th>SCONJ</th>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>5</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>74</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>50</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>3704</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>6</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <th>SYM</th>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>2</td>
      <td>8</td>
      <td>0</td>
      <td>20</td>
      <td>0</td>
      <td>0</td>
      <td>103</td>
      <td>16</td>
      <td>0</td>
      <td>1</td>
      <td>50</td>
      <td>0</td>
      <td>14</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>74</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>5</td>
      <td>0</td>
      <td>33</td>
      <td>5</td>
      <td>0</td>
      <td>0</td>
      <td>2</td>
      <td>5</td>
      <td>0</td>
      <td>52</td>
      <td>35</td>
      <td>16</td>
      <td>0</td>
      <td>0</td>
      <td>7</td>
      <td>57</td>
      <td>1</td>
      <td>90</td>
      <td>0</td>
      <td>1</td>
    </tr>
    <tr>
      <th>VERB</th>
      <td>19</td>
      <td>1420</td>
      <td>1731</td>
      <td>3260</td>
      <td>8</td>
      <td>663</td>
      <td>67</td>
      <td>29</td>
      <td>39</td>
      <td>166</td>
      <td>2</td>
      <td>0</td>
      <td>1776</td>
      <td>47</td>
      <td>1</td>
      <td>3037</td>
      <td>0</td>
      <td>261</td>
      <td>4</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>9</td>
      <td>0</td>
      <td>0</td>
      <td>8</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>12</td>
      <td>8</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>13</td>
      <td>0</td>
      <td>0</td>
      <td>19</td>
      <td>10</td>
      <td>2</td>
      <td>0</td>
      <td>4</td>
      <td>892</td>
      <td>0</td>
      <td>5</td>
      <td>7324</td>
      <td>0</td>
      <td>2243</td>
    </tr>
    <tr>
      <th>X</th>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>48</td>
      <td>6</td>
      <td>49</td>
      <td>0</td>
      <td>0</td>
      <td>5</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>49</td>
      <td>0</td>
      <td>43</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>12</td>
      <td>257</td>
      <td>0</td>
      <td>57</td>
      <td>0</td>
      <td>7</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>1</td>
      <td>0</td>
      <td>114</td>
      <td>3</td>
      <td>15</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>7</td>
      <td>3</td>
      <td>0</td>
      <td>165</td>
      <td>0</td>
      <td>0</td>
    </tr>
  </tbody>
</table>


### Create a chainable search method

```python

def searcher(df, column, query, inverse=False):
    """Search column for regex query"""
    bool_ix = df[column].str.contains(query)
    return df[bool_ix] if not inverse else df[~bool_ix]

import pandas as pd
pd.DataFrame.search = searcher

# get nominal subjects
df.search('f', 'nsubj').search('w', '^[abc]').head().to_html()
```
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th></th>
      <th>w</th>
      <th>l</th>
      <th>x</th>
      <th>p</th>
      <th>g</th>
      <th>f</th>
      <th>e</th>
      <th>type</th>
      <th>gender</th>
      <th>Case</th>
      <th>Definite</th>
      <th>Degree</th>
      <th>Foreign</th>
      <th>Gender</th>
      <th>Mood</th>
      <th>Number</th>
      <th>Person</th>
      <th>Poss</th>
      <th>Reflex</th>
      <th>Tense</th>
      <th>Voice</th>
      <th>Type</th>
      <th>gw</th>
      <th>gl</th>
      <th>gp</th>
      <th>gf</th>
      <th>count</th>
    </tr>
    <tr>
      <th>s</th>
      <th>i</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>3</th>
      <th>4.0</th>
      <td>authorities</td>
      <td>authority</td>
      <td>NOUN</td>
      <td>NNS</td>
      <td>5</td>
      <td>nsubj</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Plur</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>announced</td>
      <td>announce</td>
      <td>VBD</td>
      <td>parataxis</td>
      <td>1</td>
    </tr>
    <tr>
      <th>8</th>
      <th>2.0</th>
      <td>cells</td>
      <td>cell</td>
      <td>NOUN</td>
      <td>NNS</td>
      <td>4</td>
      <td>nsubj</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Plur</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>operating</td>
      <td>operate</td>
      <td>VBG</td>
      <td>root</td>
      <td>1</td>
    </tr>
    <tr>
      <th>9</th>
      <th>3.0</th>
      <td>announcement</td>
      <td>announcement</td>
      <td>NOUN</td>
      <td>NN</td>
      <td>6</td>
      <td>nsubj:pass</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Sing</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>made</td>
      <td>make</td>
      <td>VBN</td>
      <td>advcl</td>
      <td>1</td>
    </tr>
    <tr>
      <th rowspan="2" valign="top">12</th>
      <th>3.0</th>
      <td>commander</td>
      <td>commander</td>
      <td>NOUN</td>
      <td>NN</td>
      <td>7</td>
      <td>nsubj</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Sing</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>announced</td>
      <td>announce</td>
      <td>VBD</td>
      <td>root</td>
      <td>1</td>
    </tr>
    <tr>
      <th>9.0</th>
      <td>bombings</td>
      <td>bombing</td>
      <td>NOUN</td>
      <td>NNS</td>
      <td>11</td>
      <td>nsubj</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>Plur</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>_</td>
      <td>declined</td>
      <td>decline</td>
      <td>VBN</td>
      <td>ccomp</td>
      <td>1</td>
    </tr>
  </tbody>
</table>


### Create a concordancer

```python
def _conclines(match, df=False, column=False):
    """Apply this to each sentence"""
    s, i = match.name
    sent = df['w'].loc[s]
    match['left'] = sent.loc[:i].str.cat(sep=' ')
    match['right'] = sent.loc[i:].str.cat(sep=' ')
    formatted = match['w']
    if column != 'w':
        formatted += '/' + match[column]
    match['match'] = formatted
    return match

def conc(df, column, query):
    """Build simple concordancer"""
    # get query matches
    matches = df[df[column].str.contains(query)]
    # add left and right columns
    lines = matches.apply(_conclines, df=df, column=column, axis=1)
    return lines[['left', 'match', 'right']]

import pandas as pd

pd.DataFrame.conc = conc
lines = df.head(1000).conc('l', 'be')
lines.head(10).to_html()
```

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th></th>
      <th>left</th>
      <th>match</th>
      <th>right</th>
    </tr>
    <tr>
      <th>s</th>
      <th>i</th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2</th>
      <th>9.0</th>
      <td>[ This killing of a respected cleric will be</td>
      <td>be/be</td>
      <td>be causing us trouble for years to come . ]</td>
    </tr>
    <tr>
      <th rowspan="2" valign="top">4</th>
      <th>4.0</th>
      <td>Two of them were</td>
      <td>were/be</td>
      <td>were being run by 2 officials of the Ministry ...</td>
    </tr>
    <tr>
      <th>5.0</th>
      <td>Two of them were being</td>
      <td>being/be</td>
      <td>being run by 2 officials of the Ministry of th...</td>
    </tr>
    <tr>
      <th rowspan="4" valign="top">5</th>
      <th>5.0</th>
      <td>The MoI in Iraq is</td>
      <td>is/be</td>
      <td>is equivalent to the US FBI , so this would be...</td>
    </tr>
    <tr>
      <th>15.0</th>
      <td>The MoI in Iraq is equivalent to the US FBI , ...</td>
      <td>be/be</td>
      <td>be like having J. Edgar Hoover unwittingly emp...</td>
    </tr>
    <tr>
      <th>27.0</th>
      <td>The MoI in Iraq is equivalent to the US FBI , ...</td>
      <td>members/member</td>
      <td>members of the Weathermen bombers back in the ...</td>
    </tr>
    <tr>
      <th>31.0</th>
      <td>The MoI in Iraq is equivalent to the US FBI , ...</td>
      <td>bombers/bomber</td>
      <td>bombers back in the 1960s .</td>
    </tr>
    <tr>
      <th rowspan="2" valign="top">6</th>
      <th>3.0</th>
      <td>The third was</td>
      <td>was/be</td>
      <td>was being run by the head of an investment firm .</td>
    </tr>
    <tr>
      <th>4.0</th>
      <td>The third was being</td>
      <td>being/be</td>
      <td>being run by the head of an investment firm .</td>
    </tr>
    <tr>
      <th>7</th>
      <th>5.0</th>
      <td>You wonder if he was</td>
      <td>was/be</td>
      <td>was manipulating the market with his bombing t...</td>
    </tr>
  </tbody>
</table>