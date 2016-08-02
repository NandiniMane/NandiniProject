# NandiniProject
This is just a test project 


import java.util.concurrent.TimeUnit;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;

public class A
{
static String driverPath = "C:/Users/a555874/Downloads/chromedriver_win32/chromedriver.exe";

public static void function(String fileName)
     {
    
		System.out.println("Launching google chrome with new profile..");
		System.setProperty("webdriver.chrome.driver", driverPath);
		driver = new ChromeDriver();
	    driver.manage().timeouts().implicitlyWait(200, TimeUnit.SECONDS);
		baseUrl = "https://c360console-qa.fmr.com/C360Console/app/landingPage";
	    driver.get(baseUrl);
	    driver.manage().window().maximize(); 
	    System.out.println("Success");
}
}

