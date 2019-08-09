# Selenium - how to
```java
// go somewhere on the web
driver.get("http://www.my.url");

// check page title
String s = driver.getPageTitle();

// get a DOM node text
WebElement el = driver.findElement(By.id("elementID"));
el.getText();

// fill in a form
WebElement select = driver.findElement(By.tagName("select"));
List<WebElement> selectOptions = selet.findElements(By.tagName("option"));
for (WebElement option : allOptions) {
  System.out.println(String.format("Value: %s", option.getAttribute("value")));
  option.click();
}

Select select = new Select(driver.findElement(By.tagName("select")));
select.deselectAll();
select.selectByVisibleText("some text");
```
