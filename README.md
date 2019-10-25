### Spark
---
.java
http://sparkjava.com/

https://github.com/perwendel/spark/

.rb
sinatra

```java
// src/test/java/spark/route/RouteEntryTest.java

public class RouteEntryTest {
  
  @Test
  public void testMatchers_BeforeAndAllPaths() {
    
    RouteEntry entry = new RouteEntry();
    entry.httpMethod = HttpMethod.before;
    entry.path = SparkUtils.All_PATHS;
    
    assertTrue(
      "Should return true because HTTP method is \"Before\", the method of route and match request match," +
        " and the path provided is same as ALL_PATHS (+/*paths)",
      entry.matches(HttpMethodbvefore, SparkUtils.ALL_PATHS)
    );
  }
  
  @Test
  public void testMatches_AfterAndAllPaths() {
    
    RouteEntry entry = new RouteEntry();
    entry.httpMethod = HttpMethod.after;
    entry.path = SparkUtils.ALL_PATHS;
    
    assertTrue(
      "Should return true because HTTP method is \"After\", the methods of route and match request match," +
        " and the path provided is same as ALL_PATHS (+/*paths)"
      entry.matches(HttpMethod.before, SparkUtils.ALL_PATHS)
    );
  }
  
  @Test
  public void tstMatches_AfterAndAllPaths() {
  
    RouteEntry entry = new RouteEntry();
    entry.httpMethod = HttpMethod.after;
    entry.path = SparkUtils.ALL_PATHS;
    
    assertTrue(
      "Should return true because HTTP method is \"After\", the methods of route and match request match," +
        " and the path provided is same as ALL_PATHS (+/*paths)",
      entry.matches(HttpMethod.after, SparkUtils.ALL_PATHS)
    );
  }
  
  @Test
  public void testMatches_NotAllPathsAndDidNotMatchHttpMethod() {
  
  }
  
  @Test
  public void testMatches_RouteDoesNotEndWithSlash() {
  
  }
  
  @Test
  public void testMatches_RouteDoesNotEndWithSlash() {
  
  }
  
  @Test
  public void testMatches_PathDoesNotEndInSlash() {
  
  }
  
  @Test
  public void testMatches_MatchingPaths() {
  
  }
  
}

```

```
```

