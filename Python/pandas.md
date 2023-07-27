`import pandas as pd`

`df = pd.read_csv()`

`type(df)`

`df.shape`

`df.columns`

`df.dtypes`

`df.info()`

`df.head()`

`df.tail()`

`df['country']`

subset need `[[...]]`
- outer `[]` tells subset
- inner `[]` tells lists of columns
- subset = df[['country', 'year']]

Cannot pass index in dataframe.  if you want, `.iloc[]` notation needed.

"Series" object is from a single columns from dataframe
- country_df = df['country']

"list" object is from double blanket `[[...]]`
- country_df_list = df[['country']]

"." Dot notation is available
- df.country

  subset row
  - loc[] can not allow `df.loc[-1]`
  - .iloc[] can allow `df.iloc[-1]`

 `df.head(n=1)` is pandas

 `df.loc[0]` is series

 slice
 - `df.loc[:, ['year`, 'pop']`
 - `df.iloc[:, [2, 4, -1]]`
 - `df.iloc[:, 3:6]`
 - multiple row and column `df.iloc[[0,99,999], [0, 3, 5]]`

subsetting with `range()`
- `df.iloc[:, list(range(0,1,2,3,4))]`

group by `df.groupby('year').mean()`

flatten data `df.reset_index()`

Grouped Frequency Counts `df.groupby('continent')['country'].nunique()`

