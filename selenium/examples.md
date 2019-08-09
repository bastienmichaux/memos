# Selenium - Examples
Example test:
```java
package org.openqa.selenium.example;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.firefox.FirefoxDriver;
import org.openqa.selenium.support.ui.ExpectedCondition;
import org.openqa.selenium.support.ui.WebDriverWait;

public class Selenium2Example  {
  public static void main(String[] args) {
    WebDriver driver = new FirefoxDriver();
    driver.get("http://www.my.url");
    //check page title
    String title = driver.getTitle();
    // find text input element by name
    WebElement elem = driver.findElement(By.name("q"));
    elem.sendKeys("cheese");
    elem.submit();
    // wait for the page to load results after 10s
    (new WebDriverWait(driver, 10)).until(new ExpectedCondition<Boolean>() {
      public Boolean apply(WebDriver d) {
        return d.getTitle().toLowerCase().startsWith("cheese");
      }
    });
    // get page title again, should start with
    title = driver.getTitle();
    // stop test
    driver.quit();
  }
}
```
