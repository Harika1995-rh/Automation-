The below code shows how it launch the Chrome by using selenium webdriver

import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;


public class Launch_Chrome {
public static void main(String[] args) 
{
	//setting the property for chrome driver 
	System.setProperty("webdriver.chrome.driver", "C:\\Seleniumjar and drivers\\chromedriver.exe");
	//Initializing the Chrome webdriver
	WebDriver driver = new ChromeDriver();
	driver.get("https://www.facebook.com/");
	//to get the title of page
	System.out.println(driver.getTitle());
	// to close the chrome driver we use
	driver.close();
	
}
}
