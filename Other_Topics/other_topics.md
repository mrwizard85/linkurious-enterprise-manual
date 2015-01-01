# Other Topics

## Indexation

The graph database is automatically indexed on startup at the moment, you can edit this setting in linkurious/config/production.js.

Change ```force_reindex: true``` to ```force_reindex: false```.

## Requirements

Windows, Linux or Mac OS

64 bits system

Java 8u25 **and the JAVA_HOME environment variable set up** ([see how to do it on Windows](http://help.virtocommerce.com/support/discussions/topics/38969))

Neo4j 1.9.5+ or 2.x with a small database of less than 200k nodes and relationships

Internet Explorer 10, Firefox 15, Chrome 23, Safari 6, and Opera 12.

## Reportings bugs

This early version is released for **beta testing**, so please experiment with these features and report bugs at support@linkurio.us (it will open a thread on [Freshdesk](http://freshdesk.com/)).

Reported bugs will be fixed progressively.

## Importing data

Linkurious relies on Neo4j to store the data. The data importation is thus not handled by our solution. If you want to import data to Neo4j, you have those solutions:

* there is a Gephi plugin that lets you export any file compatible with Gephi to Neo4j ([list of compatible formats](https://gephi.org/users/supported-graph-formats/))

* if you can handle a spreadsheet, you can [easily](http://blog.neo4j.org/2013/03/importing-data-into-neo4j-spreadsheet.html) import csv formated data

* for the more tech savvy there are even more option ([Batch importer](https://github.com/jexp/batch-import), [Talend connector](https://github.com/Zenika/talend-neo4j-connector))

* if you want to get help from professionals, we can get you in touch with great people.

* If you are still not sure about whether you can get your data in Linkurious contact us, we’ll be happy to answer if you contact us.
*

Finally, if you want to quickly try to use Linkurious Enterprise with dummy data, you can download a [Neo4j compatible dataset](http://neo4j.com/developer/guide-example-data/).

## Overall architecture

![architecture](http://linkurio.us/wp-content/uploads/2012/12/Linkurious-architecture.png)

Linkurious is the sum of two components: the frontend, running in the web browser and providing the user interface, and the backend, server component connected to the graph database. The backend provides a fast search engine and runs on any system able to support node.js, including Windows, Linux and Mac OS.

While we ship a lightweight search engine fully running in memory, it can easily be switched to another engine such as Apache Lucene. The graph database can be located on the same machine as the backend or on any other machine in your network.

## Technology

Below is a list of the open source technologies we use. They have proven to be efficient and reliable:

* [Angular.js](https://angularjs.org/)
* [Sigma.js](http://sigmajs.org/)
* [ElasticSearch](http://www.elasticsearch.org/)
* [Node.js](http://nodejs.org/)

