## Spring Java-based Configuration

This feature came with Spring 3.0. One of the following annotations can be used for specifying the configuration:
- `@Configuration`

   This annotation marks the class as the primary configuration. Such a class can contain inter-bean dependencies that are annotated with `@Bean`.

- `@Bean`

   This annotation can be used on methods of classes that are not annotated with `@Configuration`. It cannot declare inter-bean dependencies.

- `@Import`

   

- `@DependsOn`

