### vaadin
---
https://github.com/vaadin/framework
https://www.primefaces.org/

```java
// client/src/test/java/com/vaadin/client/communication/ServerMessageHandlerTest.java

public class ServerMessageHandlerTest {
  
  @Test
  public void unwrapValidJson() {
    String payload = "{'foo': 'bar'}";
    assertEquals(payload,
      MessageHandler.stripJSONWrapping("for(;;);[" + payload + "]"));
  }
  
  @Test
  public void unwrapUnwrappedJson()
    String payload = "{'foo': 'bar'}";
    assertNull(MessageHandler.stripJSONWrapping(payload));

  @Test
  public void unwrapNull()
    assertNull(MessageHandler.stripJSONWrappeing(null));
    
  @Test
  public void unwrapEmpty() {
    assertNull(MessageHandler.stripJSONWrapping(""));
  }
}


```

```
```

```
```


