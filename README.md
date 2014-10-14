# csvigo: a package to handle CSV files (read and write).
This ia a clone of clementfarabet/lua---csv.  

## Install:

Install clementfarabet/lua--csv per the instructions, replace init.lua
and README.md with those found here.

## Use:

The library provides 3 high-level functions: csvigo.load, csvigo.save
and csvigo.ordered_save. To get help
on these functions, simply do:

```
> help(csvigo.save)
> help(csvigo.load)
> help(csvigo.ordered_save)
```

Loading a CSV file in 'query' mode gives you a convenient query function that
you can use to query subsets of your original CSV file. To get help on this query
function, simply do:

```
> query = csvigo.load{path='somefile.csv', mode='query'}
> query('help')
-- print some help
> all = query('all')
> subset = query('union', {somevar=someval, someothervar={val1, val2}})
