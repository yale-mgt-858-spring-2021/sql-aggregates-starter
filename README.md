# 

In this assignment we'll continue practicing with joins and aggregates.
We'll be using the `pagila` schema in the class database. The tables
in the schema model a DVD rental store. Remember those!? 🤣 If you 
drive down Whitney you'll still find one in operation:  [Best Video](https://www.courant.com/ctnow/movies/hc-best-video-in-hamden-20160529-story.html).
Though, it is no longer a video store, but rather
[a non-profit video archive](https://www.connecticutmag.com/arts/hamdens-best-video-no-longer-a-video-store-but-better/article_0659c0d0-c2f0-11e6-96be-5fd6fe69a422.html),
coffee shop, and music venue.
It's a great place to visit!

Well, the `pagila` schemas holds movies (mostly older movies), customer,
employees, stores (locations), rentals, payments, and related data.
We're going to use these tables to answer some of the kinds of questions
in which management might be interested.  In all cases, please pay 
attention to column names and sort order!

As ever, when I inevitably find errors in this assignment, or parts of
the assignment that need clarification, I will post in slack and update
this starter code. (Of course, if you've already started, you won't see
my updates automatically! You'll have to check Slack.) I'll also update
this description on the class website.

To get started, [accept this GitHub Classroom invite](https://classroom.github.com/a/nUxHd1YZ)
and then paste your repo URL in the class website.

## Updates on Sun Apr  4
Various updates based on feedback from Jean Chen.

## Updates on Mon Apr  5 08:54:12 EDT 2021
Updates based on feedback from Gary Yan.

* **Q1 Actor Names**: The Readme.md file is missing formatting for last_name and first_name in the second last sentence of the file; (*CHANGED*)
* **Q4 Staff Payments**: Not sure how explicit you want your instructions to be, but I had to also sort the names by alphabetical to match my answer with the example table; (**CHANGED**, but I also need to get my grading working such that for some questions order does not matter.)
* **Q6 Film Inventory**: Does not name the tables to use for the SQL query, but assumed to be a JOIN of the tables film and inventory; (**CHANGED**)
* **Q10 Most Popular**: Unless I'm misunderstanding something, I think you also need to JOIN the rental table as well? The payment table only contains rental_id and that needs to be converted into a category_id based on the chain rental_id -> inventory_id -> film_id -> category_id; (**CHANGED**, that is correct, though in the future I will not specify what tables are needed because it ought to be obvious from the schema.)
* **Q11 Rental Statistics**: Is it a problem if the format Datagrip gives the answer in is a different format to what is in the example table? I assume this is a settings thing and not a data output issue. (This is not a problem. Your query will be run in a PostgreSQL client that is *not* Datagrip, so as long as your query is matches hime we should be fine.)


## Suggested order

We suggest you complete the questions in the following order

- [ ] 00-actors-with-letter-a
- [ ] 01-actor_names
- [ ] 02-actor_names_count
- [ ] 03-staff-addresses
- [ ] 04-staff-payment-total
- [ ] 05-count-ratings
- [ ] 06-film-inventory-count
- [ ] 07-count-film-actors
- [ ] 08-total-custom-payments
- [ ] 09-most-rented-movies
- [ ] 10-most-popular-genres
- [ ] 11-rental-return-stats


As you complete questions, you can mark them as complete
in this Markdown file,  but you don't have to do so.
See [this example](https://github.blog/2014-04-28-task-lists-in-all-markdown-documents/).

