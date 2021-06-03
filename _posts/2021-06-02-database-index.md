---
layout: post
title: Database Index
excerpt: "Database Index (PostgreSQL)"
categories: [Daily]
tags: [TIL, database]
comments: true
image:
  feature:
  credit: 
  creditlink: 
---

## Database Index (PostgreSQL)

I discovered this today at work. A few weeks ago, we have a problem with selecting rows in one of the tables we use in the database was super slow that causes an issue. The table contained about 5 million rows this selecting rows process shouldn't take that long. 

My colleague brought a good idea that we can create an index for the column we used to select in the table. Our team agreed to use that method and it worked out well.

I kinda knew what is database index cons and pros from class in University but never had a chance to experience it. 

Today, I had to delete 8 rows from a table that has about 6000 rows and it took about 7 seconds to delete the rows! This is one of the cons of indexing a database. When you indexing the database, you can select it faster but insert/update/delete operations will be slow! and that table had 3 indexes created. 

It is amazing to see something you learned from the paper and see it in the field. Now, I know that this will gives me a good memory to memorize this longer. Thank you, my co-workers!