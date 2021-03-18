
The `minimum_nights` column of the `stays` table indicates the minimum
number of nights that the occupant was required to book for a particular
stay. A value of 2 means that the occupant was required to stay for at
least 2 nights. Imagine that we'd like to know in which neighborhoods
multi-night stays are concentrated.  Produce a list of neighbourhood
groups and neighbourhoods that have 10 or more stays that required more
than a single night's occupancy. Sort the results in descending order by
the number of multi-night stays.  You'll want to use `GROUP BY`, `HAVING`
and `ORDER BY`.  Your results should look something like this (these
might not be correct results). 

```
neighbourhood_group |   neighbourhood    | multinight_stays
---------------------+--------------------+------------------
 Brooklyn            | Williamsburg       |               20
 Manhattan           | Harlem             |               18
 Manhattan           | East Village       |               12
 Manhattan           | Hell's Kitchen     |                9
(4 rows)
```

In the example results above, I am showing that Brooklyn's Williamsburg
neighbourhood has 20 stays on record each of which required more than
a single night. Harlem had 18 such stays.