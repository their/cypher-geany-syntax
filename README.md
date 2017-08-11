Cypher Geany Syntax
=================

What is it?
-----------
This is a basic [Geany] syntax for the awesome [Cypher](http://docs.neo4j.org/chunked/stable/cypher-query-lang.html) graph database query language.  Cypher is like SQL for graph databases.  You can find Cypher on [Neo4j](http://www.neo4j.org).

Why should I use it?
--------------------

Because syntax highlighting is really helpful, that's why.  Also, we want people to be able to do ad-doc queries and graph updates in their favourite shell, and not compromise readability, etc.

How should I use it?
--------------------

* git clone git://github.com/their/cypher-geany-syntax.git
* cd cypher-geany-syntax/ && cp filetypes.Cypher.conf .config/geany/filedefs/
* Edit filetype_extensions.conf: (Tools->Configuration Files->filetype_extensions.conf)
* Under [Extensions] add: Cypher=*.cyp;*.cypher;
* Edit a file that has the extension **.cyp** or **.cypher**

Who should I thank?
-------------------

* [robinedwards](https://github.com/robinedwards) for extending the syntax.
* [their](https://github.com/their) for extending to geany.

Todo
----
Add the following equivalents in geany:
* -syn region    cypherProperty      start=+'+ skip=+\\\\\|\\'+ end=+'+
* -syn match     cypherRelationship  ":\w*_\w*"
* -syn match     cypherSymbol        "->"
* -syn match     cypherSymbol        "<=>"
* -syn match     cypherSymbol        "<-"
* -syn match     cypherPropertyName  "\w\+:"
* -syn match     cypherVariable      "\w\+"

Thanks guys!
