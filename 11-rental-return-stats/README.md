
We'd like some stats on how long rentals are out for. Please
use the `rental` table to analyze the difference between the
`return_date` and `rental_date`.  Your results should look like as follows.
The `p25` column is the 25th percentile, `p50` is the 50 percentile
(the median). You might want to use the [percentile_disc](https://leafo.net/guides/postgresql-calculating-percentile.html)
function to compute these.
Your results should look like this. Though, Datagrip may give you slightly
different formatting to what you see here. I'm using the `psql` client
and I'm told it has different looking output thann Datagrip. If you
have the right query, it won't matter.

```
│          avg           │   min    │       max       │       p25       │       p50       │       p75       │      p100       │
├────────────────────────┼──────────┼─────────────────┼─────────────────┼─────────────────┼─────────────────┼─────────────────┤
│ 4 days 24:36:28.541706 │ 18:00:00 │ 9 days 05:59:00 │ 2 days 20:52:00 │ 5 days 00:34:00 │ 7 days 03:29:00 │ 9 days 05:59:00 │
```