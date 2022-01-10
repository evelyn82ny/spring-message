## Message

하드 코딩을 피하기 위해 message 기능을 사용한다.<br>

```properties
<h2>상품 수정</h2>
<h2 th:if="${param.status}">저장 완료</h2>
```

위와 같이 하드 코딩할 경우 수정할 부분을 일일이 수정해야 한다.<br>

```properties
<h2 th:text="#{page.updateItem}">상품 수정</h2>
<h2 th:if="${param.status}" th:text="#{page.saved}">저장 완료</h2>
```

하지만 위와 같이 message 기능을 사용하면 **message.properties** 파일만 수정하면 된다.<br>

- message.properties : default
- message_en.properties : english


