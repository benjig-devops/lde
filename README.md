
Lead Data Engineer Interview Task, Lavamap
==========================================

Algorithm for Nightly Script
-------------------------------

1. Pull list of domains by domain substring via API, given substring of "lava."
2. Pull current list of domains for that substring, where 'deleted\_at' IS NULL.
3. Determine changes to our database:
	1. Domains in the list from the API but not in the current list are added.
	2. Domains in the current list but not the API are deleted.
4. Log if no domains are added, if no domains are deleted.

Feedback/Notes on Solution
----------------------------

1. Apologies for the delay on delivery, a couple things contributed to it:
	1. Setting up a postgres database server was new to me, but after that the database was familiar.
	2. I spent a bit of time trying to figure out if I was missing something on the API limitations.
	3. End of the month reports took a little more time than I expected.
2. I added the second table to make the database a little more general.
