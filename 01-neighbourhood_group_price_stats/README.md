
We'd like to compute some price stats for each 
neighbourhood group in the `airbnb_ny.stay` table.
Please create a table like that you see below. (I suspect
the columns are self-explanatory.)

```
│ neighbourhood_group │ num_listings │      avg_price       │    stddev_price     │ min_price │ max_price │
├─────────────────────┼──────────────┼──────────────────────┼─────────────────────┼───────────┼───────────┤
│ Queens              │           11 │ 146.0909090909090909 │ 87.7649754121250187 │        55 │       350 │
│ Brooklyn            │          111 │ 137.4594594594594595 │ 96.0873450927742460 │        35 │       800 │
│ Staten Island       │            2 │  53.0000000000000000 │ 24.0416305603426158 │        36 │        70 │
│ Manhattan           │          124 │ 151.8467741935483871 │ 87.5397279710727106 │        40 │       500 │
│ Bronx               │            2 │  42.5000000000000000 │  3.5355339059327376 │        40 │        45 │
```