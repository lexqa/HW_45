# HW_45

package core;

import org.openqa.selenium.WebDriver;

public class Main {

	static WebDriver driver;

	public static void main(String[] args) throws Exception {
		SignUp.validate(driver, "http://abc.com/login");
		Common.quit();
		Confirmation.validate(driver, "http://abc.com/confirmation.php");
		Common.quit();
	}
}
