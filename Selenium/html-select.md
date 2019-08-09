# Selenium - HTML Select
```java
// deal with <select> elements
Select select = new Select(driver.findElement(By.tagName("select")));
select.deselectAll();
select.selectByVisibleText("some text");
```
