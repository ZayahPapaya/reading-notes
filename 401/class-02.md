# Class 2

[401 Home](../home401.md)

## NodeJS & Express

- Middleware is the tool by which you connect two systems together. Client to server, server to server, server to database.
- Express is the most popular Node web framework.
- Express is unopinionated in that it is not made in a way to enforce a particular style of code or structure. It's simply a tool that can be used however you'd prefer.
- A module is a batch of code that can be imported over into other files as a library.

## NPM (Node package manager)

- I am using NPM 6.14.16
- `npm i jshint`

## TDD (Test driven developmment)

- Writing tests (especially first) forces you to write better, cleaner code with clear inputs and outputs. You also get a sort of pulse on how healthy your code is as you're working on it.
- "many teams report significant reductions in defect rates, at the cost of a moderate increase in initial development effort", "the same teams tend to report that these overheads are more than offset by a reduction in effort in projects’ final phases", "although empirical research has so far failed to confirm this, veteran practitioners report that TDD leads to improved design qualities in the code, and more generally a higher degree of “internal” or technical quality, for instance improving the metrics of cohesion and coupling" 
[Agile Alliance](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1))
- Individual pitfalls: Not testing often, writing too many tests, writing tests that are too narrow or too broad.
- Team pitfalls: Only partial use of TDD, poor maintenance of testing, abandoned testing.

## CI/CD (Continuous integration & Continuous deployment)

- Ensures integration ease, catches bugs, reduces conflicts.
- Continuous delivery is developing to be ready to release at any time, continuous deployment is deploying features immediately with little downtime.
- Github manages automated testing for different integrations.
