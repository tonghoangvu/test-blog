# test-blog

```HelloWorld.java
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello World!");
  }
}
```

```java
@Component
public class TomcatServerCustomizer
    implements WebServerFactoryCustomizer<TomcatServletWebServerFactory> {
  @Override
  public void customize(TomcatServletWebServerFactory factory) {
    factory.addContextCustomizers(
        context -> {
          if (context.getParent() instanceof StandardHost standardHost) {
            standardHost.setErrorReportValveClass(NoOpErrorReportValve.class.getName());
          }
        });
  }

  public static class NoOpErrorReportValve extends ErrorReportValve {
    @Override
    protected void report(Request request, Response response, Throwable throwable) {}
  }
}
```

## Table of Contents

- [ ] Check item 1
- [x] Check item 2
- [ ] None

[DEMO 1](./demo-1)
[DEMO 1 MD](./demo-1.md)
