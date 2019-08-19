## A simple HTTP API

### Objective

We define a mock JSON HTTP API for a minimalist job board
application. The API exposes the following routes:

- `GET /jobs`: Returns a map of open positions in the job board.
- `POST /jobs`: Inserts a new open position in the job board and
  returns the updated map.
- `DELETE /jobs/:id`: Removes an open position from the job board and
  returns the updated map.

Job IDs should be textual representations of UUIDs. Jobs should have
a `company`, `title`, and `description` field.

### Assignment details

The project should be delivered as an [sbt](https://www.scala-sbt.org/)
project, starting the API server on `localhost` port `9000` when
launched with `sbt run`.

Storage of jobs should be limited to in-memory, and functional
boundaries should be split across clearly defined components within
the daemon.

No automated tests will be ran on our side, and attention will be given to choices
made in terms of dependencies and code architecture. 

### Follow-up questions

- Describe security concerns with the code you've provided. 
- Imagine your code quickly become extremely popular, and people is posting a massive amount of jobs per minute. What piece of architecture would you add?
- 
