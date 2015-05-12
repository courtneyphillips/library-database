
#Library Database

---

_Please note that library database is still a work in progress, and is therefore not yet in a functional state._

## Synopsis

Library Database is a work-in-progress by [Courtney Phillips](https://github.com/courtneymaepdx) and [Ian Bevel](https://github.com/ianofearth) aimed at mimicking the functionality of a library database system with the ability to track patrons, maintain and query catalogues of books, and record lended books, due dates, etc. Crafted as part of the Spring 2015 Ruby course curriculum at [Epicodus](https://www.epicodus.com/).

## Database Setup

```
# psql
username=# CREATE DATABASE library;
username=# \c library;
hair_salon=# CREATE TABLE patrons (id serial PRIMARY KEY, name varchar);
hair_salon=# CREATE TABLE books (id serial PRIMARY KEY, title varchar, genre varchar, author varchar);
hair_salon=# CREATE TABLE books_patrons (id serial PRIMARY KEY, book_id int, patron_id int);
hair_salon=# CREATE DATABASE library_test WITH TEMPLATE library;
```

## Contribute

  - Issue Tracker: https://github.com/courtneyphillips/library-database/issues
  - Source Code: https://github.com/courtneyphillips/library-database
  - Pull Requests: https://github.com/courtneyphillips/library-database/pulls

## Installation

Library Database uses the following gems:

  - Capybara
  - Sinatra
  - Sinatra-Contrib
  - RSpec
  - Pry
  - PG

To install, run `gem install bundle` in the command line.

## Tests

Both method and integration tests for Library Database utilize the RSpec. Simply run `gem install rspec`, if it's not already installed, simply issue the command `rspec`, while located in the project's file.

## Links

  - GitHub: https://github.com/courtneyphillips/library-database

## Contact

Questions, concerns, fan-mail, or other grievances can be directed to Courtney at <courtney.mae.phillips@gmail.com>.

## License

The MIT License (MIT)

Copyright (c) 2015 Courtney Phillips

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

---
