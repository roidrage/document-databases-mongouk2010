!SLIDE

# Diversity #

!SLIDE

# The Right Tool™ #

!SLIDE

# NoSQL is about choice. #

<p class="caption"><a href="http://talks.jan.io/buzzwords-2010.html#present">Jan Lehnardt, 2010</a></p>

!SLIDE

## Not every tool is right for every job. ##

!SLIDE

## Relational databases are the best proof. ##

!SLIDE

## MongoDB is not alone. ##

!SLIDE bullets incremental

## Document Databases ##

* CouchDB
* MongoDB
* Riak

!SLIDE

## Same but different. ##

!SLIDE bullets incremental

# CouchDB #

* Made of the web
* Uses HTTP, JSON, JavaScript
* Queries using Map/Reduce
* P2P-like replication

!SLIDE bullets incremental

# Riak #

* HTTP interface
* Simple data model
* Instant scale out, just add more nodes 

!SLIDE bullets incremental

# MongoDB #

* BSON (binary JSON)
* Dynamic queries
* Index support
* Atomic operations on data

!SLIDE

# MongoDB #

## Relational databases meet the web. ##

!SLIDE

# Differences #

!SLIDE

# Querying Data #

!SLIDE bullets incremental

# CouchDB #

* Map/Reduce
* Precalculated views
* Built using JavaScript or Erlang
* Brain-twisting

!SLIDE bullets incremental

# Riak #

* Map/Reduce
* Calculated on demand
* Built using JavaScript or Erlang

!SLIDE bullets incremental

# MongoDB #

* Dynamic queries
* SQL-ish
* Secondary Indexes

!SLIDE

# MongoDB's Edge: #

!SLIDE

# Flexible Query Model #

!SLIDE

# Ad-hoc Queries #

!SLIDE

# Scaling Out #

!SLIDE bullets incremental

# CouchDB #

* Replicate anywhere, anytime
* P2P

!SLIDE bullets incremental

# Riak #

* Hash ring cluster
* No special nodes
* Nodes can be added any time
* Scales up with added nodes

!SLIDE

# MongoDB #

* Replication
* Replica Sets
* Auto-sharding

!SLIDE bullets incremental

# Replication #

* Initial sync
* Stream changes from master (opslog)
* Big improvement over MySQL replication

!SLIDE bullets incremental

# Replica Sets #

* TODO!

!SLIDE center

# Auto-Sharding #

![MongoDB's Auto-Sharding](mongodb_sharding.png)

!SLIDE bullets incremental

# Auto-Sharding #

* Config servers
* Routing processes
* Shards (Replica Sets)
* Lots of moving parts

!SLIDE 
