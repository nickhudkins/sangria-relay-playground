## Sangria-relay playground

This is an example of [GraphQL](https://facebook.github.io/graphql) server supporting [Relay](https://facebook.github.io/relay/) written with [Play framework](https://www.playframework.com) and [Sangria](http://sangria-graphql.org), it also uses [webpack](https://webpack.github.io/) for client side asset generation.
 
This example is based on the [Relay Star Wars example](https://github.com/facebook/relay/tree/v0.9.0/examples/star-wars). You can find more info [here](https://facebook.github.io/relay/docs/en/graphql-server-specification.html).

It also serves as a playground - on the right hand side you see a textual representation of the GraphQL
schema which is implemented on the server and that you can query here. On the left hand side
you can execute a GraphQL query and see the results of its execution.

It's available here:

[http://try-relay.sangria-graphql.org](http://try-relay.sangria-graphql.org)

This is just a small demonstration. It really gets interesting when you start to play with the schema on the server side. Fortunately it's
pretty easy to do. Since it's a simple Play application using webpack, all it takes to start playground locally and start playing with the schema is this:

```bash
$ git clone https://github.com/sangria-graphql/sangria-relay-playground.git
$ cd sangria-relay-playground
$ npm install
$ sbt run
```

Now you are ready to go to [http://localhost:9000](http://localhost:9000) for the playground or to [http://localhost:9000/starwars](http://localhost:9000/starwars) for the minimal Star Wars example.

The prerequisites are [SBT](http://www.scala-sbt.org/download.html), [Java 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html), [npm](https://www.npmjs.com/), [babel](https://babeljs.io/) and [webpack](https://webpack.github.io/).
