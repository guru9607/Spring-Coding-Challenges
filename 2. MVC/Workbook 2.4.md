# Workbook 2.4

![Screen Shot 2022-08-15 at 11.15.40 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F3fd2b093-8f71-4245-9398-2ba3229c22f8?alt=media&token=9ef422c6-fe7d-4adc-b68c-212ca26a54d1)

## Task 1

The path depends on a thymeleaf expression. Use `th:src` instead of `src`, and set it equal to a dynamic path. 

```s
"${condition} ? 'plain-text' : 'plain-text'"
```
**Attention**: Please wrap plain text inside an expression with single quotes.

## How Beautifully th:src dynamically changes absolute image path.  
```
<h1 th:text = "'Speed: ' + ${speed}"></h1>
<img th:src="${speed > 60} ? '@{images/slow-down.png}' : @{images/speed-limit.png}" width="200"></span>
```
