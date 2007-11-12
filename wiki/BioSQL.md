---
title: BioSQL
permalink: wiki/BioSQL
layout: wiki
---

[BioSQL](http://www.biosql.org/wiki/Main_Page) is a joint effort between
the OBF project (BioPerl, BioJava etc) to support a shared database
schema for storing sequence data. In theory, you could load a GenBank
file into the database with BioPerl, then extract this from the database
as a [SeqRecord](SeqRecord "wikilink") with featues using Biopython -
and get more or less the same thing as if you had loaded the GenBank
file directly using [SeqIO](SeqIO "wikilink").

Existing documentation for the Biopython interfaces to BioSQL cover
installing Python database adaptors and basic usage of BioSQL:
[HTML](http://biopython.org/DIST/docs/biosql/python_biosql_basic.html) |
[PDF](http://biopython.org/DIST/docs/biosql/python_biosql_basic.pdf) --
I hope to use this wiki page to update this documentation in future.

Installation
------------

This is fairly complicated. First of all, you will need to install the
relevent database client/server software and associated python interface
library. In this example we'll talk about the most common choice, MySQL,
and assume you'll be running your own database server on the same
machine (rather than for example using a networked database server
shared between a group). How you do this will depend on your operating
system, for example on a Debian or Ubuntu Linux machine try this:

sudo apt-get install mysql-common mysql-server mysql-admin
python-mysqldb

One the software is installed, your next task is to setup a database and
import the BioSQL scheme (i.e. setup the relevant tables within the
database). *To do...*

Before you start trying to load sequences into the database, it is a
good idea to load the NCBI taxonomy database using the
scripts/load\_ncbi\_taxonomy.pl script in the BioSQL package. *To do...*