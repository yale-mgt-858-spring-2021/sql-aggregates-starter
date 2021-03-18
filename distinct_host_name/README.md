
Imagine that we have a software system that will email each host with
some kind of promo based on the number of stays they had recently at
their property. We want to ensure that each host only gets one email and
each email is personalized for them. Use `GROUP BY`, `CASE`,  and the
string concatenation function `||` to create the data the email system
will need to write to hosts.

Your results should look something like this (these might not be correct
results). Notice that "stay" should have the correct plural form when
a host had more than one recent stay.

```
 host_id |        salutation         |        subject
---------+---------------------------+------------------------
  204533 | Dear Kyle                 | You had 7 recent stays
   22496 | Dear Lisel                | You had 3 recent stays
   73318 | Dear Meka                 | You had 1 recent stay
   64342 | Dear Reka                 | You had 1 recent stay
 (...)
```