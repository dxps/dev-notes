
## Enable remote JMX without security

This is a simple example of how to activate JMX when starting JVM, the case when no security exists: no authentication or SSL.

```bash
java -Dcom.sun.management.jmxremote.port=9999
     -Dcom.sun.management.jmxremote.authenticate=false
     -Dcom.sun.management.jmxremote.ssl=false 
     ... (-jar <file>.jar | Class (args))
```

