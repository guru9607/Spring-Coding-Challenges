# Workbook 2.3

![Screen Shot 2022-08-15 at 11.13.17 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fbec816aa-3011-4d66-8607-a15e5717eae5?alt=media&token=574ef2bf-a753-4e88-9851-8db5f4836163)


### What I found out while solving this?
```
<h1 th:text="'Speed' + ${speed}"></h1>
<img th:if="${speed > 60}" src="images/slow-down.png" width="200"/>
<img th:unless="${speed > 60}" src="images/speed-limit.png" width="200"/>
```

Below code doesn't work because its the relative path. Therefore, it's recommended to use absolute paths or paths relative to the /static directory when referencing static resources in Thymeleaf templates.
```

```     
<img src="../static/images/slow-down.png" th:if="${speed > 60}" width="200">
<img src="../static/images/speed-limit.png" th:unless="${speed > 60}" width="200"> -->
```
