# click
import org.openqa.selenium.By;
import org.openqa.selenium.Keys;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.firefox.FirefoxDriver;
import org.openqa.selenium.interactions.Actions;

public class Right_click {

public static void main(String args[]) throws Exception{

       WebDriver driver = new FirefoxDriver();
       driver.manage().timeouts().implicitlyWait(120,TimeUnit.SECONDS);
  driver.get("http://www.snapdeal.com/");
       driver.manage().window().maximize();
        WebElement R1 = driver.findElement(By.xpath("//a[@href='/shop/mobile?src=tn&nav_id=5']"));
      Actions builder = new Actions(driver);
       builder.contextClick(R1).sendKeys(Keys.ARROW_DOWN).sendKeys(Keys.ENTER).perform();
      builder.contextClick(hindiLanguage).sendKeys(Keys.ARROW_DOWN).sendKeys(Keys.ARROW_DOWN).sendKeys(Keys.ENTER).perform();
  driver.close();
		
	}

}
