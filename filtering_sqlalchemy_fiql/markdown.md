class: center, middle
# Advanced filtering on your API endpoints with SQLAlchemy and FIQL
## Serge Domkowski <sdomkowski@kavi.com>
.footnote-center[Presentation created using remarkjs http://remarkjs.com/]
---
.left-column[
  ## Who am I?
]
.right-column[
**Serge Domkowski.red[*]**  
*Software Architect*

I’ve been involved in making web software for about 22 years. I design and
write code, talk about code, play with my son, ride my bicycle, root for the
Timbers, drink beer, and once in a while sleep.

.footnote[.red[*] <sdomkowski@kavi.com>]
]
---
.left-column[
  ## Where do I work?
]
.right-column[
**Kavi Corporation.red[*]**   

*Our mission is to help results-driven teams share and organize complex work.*

Our customers produce high-value improvements for their organizations, their
industries, and the world.

With powerful software and focused support, Kavi enables collaborative team
work, structured workflows, and secure participation. Combining
enterprise-grade security and configurability, Kavi Workspace powers teams
from a local to a global scale, without the traditional cost and risks
associated with IT.

- 22 Employees

- 8 Engineers

.footnote[.red[*] http://www.kavi.com]
]
---
.left-column[
  ## Agenda
]
.right-column[
**During this demonstration, we’ll:**

* Pull apart the FIQL draft to find it’s strengths and weaknesses.

* Look at how SQLAlchemy applies filters.

* Investigate how this effects the strategy for parsing the FIQL expression.

* Discuss the implications of this strategy.

* Subclass SQLAlchemy’s Query class to allow filtering directly from a FIQL expression.

* If time permits, we’ll improve our API by adding sorting and pagination.
]
---
class: center, middle
# FIQL Draft Specification
### https://tools.ietf.org/html/draft-nottingham-atompub-fiql-00
---
class: center, middle
# SQLAlchemy Query Class
### http://docs.sqlalchemy.org/en/latest/orm/query.html
---
class: center, middle
# How to parse the FIQL expression?
### https://github.com/sergedomk/fiql_parser/tree/0.10
---
class: center, middle
# What are the implications of this strategy?
### https://github.com/sergedomk/fiql_parser/tree/0.11
---
class: center, middle
# Subclass SQLAlchemy’s Query class
### &lt;write code and see if it works.&gt;
---
class: center, middle
# Add sorting and pagination
### &lt;write more code and see if it works.&gt;
---
class: center, middle
# Questions?
---
.left-column[
  ## Further Reading
]
.right-column[
### FIQL Draft Specification

https://tools.ietf.org/html/draft-nottingham-atompub-fiql-00

### SQLAlchemy

http://www.sqlalchemy.org/

### FIQL Parser

https://github.com/sergedomk/fiql_parser

### FIQL Parsing Query Class

https://gist.github.com/sergedomk
]

