!SLIDE center

![MongoDB](mongodb.png)

!SLIDE

## Update relevant data independently. ##

!SLIDE center

![Document](document.jpg)

!SLIDE javascript

    @@@ javascript
    db.posts.save({
      title: "Notes on MongoDB",
      contents: "For an article in a...",
      created_at: Date(),
      tags: ['mongodb', 'nosql'],
      comments: {}
    })

!SLIDE center

![Document: Tags](document_tags.jpg)

!SLIDE javascript

    @@@ javascript

    db.posts.update(
      {name: "Notes on MongoDB"},
      {$push: {tags: 'mongodb'}}
    );

!SLIDE center

![Document: Related](document_related.jpg)

!SLIDE javascript

    @@@ javascript
    post.previous = DBRef(previousPost)

!SLIDE center

![Document: Embedded](document_embedded.jpg)

!SLIDE javascript

    @@@ javascript
    db.posts.update(
      {name: "Notes on MongoDB"},
      {
        $push: {comments:
          {
            author: "Pascal betz",
            comment: "Thanks for the great..."
          }
        }
      }
    )

!SLIDE center

# Additional metadata. #

!SLIDE javascript

    @@@ javascript
    db.posts.update(
      {name: "Notes on MongoDB"},
      {$inc: {views: 1}}
    )

!SLIDE

# Dynamic queries #

!SLIDE javascript

    @@@ javascript
    db.find({name: "Notes on MongoDB"})

!SLIDE javascript

    @@@ javascript
    db.find({$gt: {views: 10}})

!SLIDE

## Requires data to be properly indexed. ##

!SLIDE

## No other document store can do dynamic queries. ##

!SLIDE center

![Document: Contents](document_contents.jpg)

!SLIDE javascript

## Only access certain attributes: ##

    @@@ javascript
    db.find(
      {name: "Notes on MongoDB"},
      {contents: 1}
    )

!SLIDE center

![MongoDB](mongodb.png)

!SLIDE bullets incremental

## It's dead-simple to start off. ##

* And to scale up.

!SLIDE bullets incremental

## Development speed. ##

* Wheeeeee!

!SLIDE bullets incremental

## The best of both worlds: ##

* Queries and indexes from relational databases
* Schemaless documents
* Some scaling features sprinkled on top
