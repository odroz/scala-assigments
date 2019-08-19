## A Simple URL Shortener

### Objective
We want to put simple API in place that would provide our users with a URL shortener funtionality. (in a [bitly](https://bitly.com/) kind of way.)

### Requirements
Users should be able to create short URLs. Simple Analytics should be gathered per URLs. 

The API should expose the following routes: 

- `POST /url`: Create a new short URL from the URL received in JSON format
- `GET /:short`: Returns the original "long URL"
- `GET /:short/stats`: Returns simple statistics on the URL


### Assignment details

The project should be delivered as an [sbt](https://www.scala-sbt.org/)
project, starting the API server on `localhost` port `9000` when
launched with `sbt run`.

Storage of jobs should be limited to in-memory, and functional
boundaries should be split across clearly defined components within
the app.

No automated tests will be ran on our side, and attention will be given to choices
made in terms of dependencies and code architecture. 


