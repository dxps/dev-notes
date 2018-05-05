## Java 9+ - Notes

### Vert.x with Java 10

When using Java 9 or newer, I used the following module definition in `{project}/src/main/java/module-info.java` file:
```
open module accounts.service {

    requires vertx.core;
    requires vertx.web;

//    requires vertx.jdbc.client;
//    requires vertx.sql.common;
    requires java.sql;

}

```
It should be reviewed and reused later when a newer version of Vert.x will officially support Java 10 (not it depends on gRPC update).


