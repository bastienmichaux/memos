# Selenium - locators
```java
// id
WebElement x = driver.findElement(By.id('x'));

// className
List<WebElement> x = driver.findElements(By.className('x'));

// tagName
WebElement x = driver.findElement(By.name('x'));

// link text
WebElement x = driver.findElement(By.linkText('x'));

// partial link text
WebElement x = driver.findElement(By.partialLinkText('x'));

// query selector (css)
WebElement x = driver.findElement(By.cssSelector('#my-id .my-class p'));

// using XPath
WebElement x = driver.findElements(By.xpath('//input'));

// using JS (wtf my dude)
WebElement x = (WebElement) ((JavascriptExecutor)driver)
  .executeScript("return $('x')[0]")
```
