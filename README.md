
# Using this Project

This project is using the latest Selenium Bindings.

## Setup

Run these commands depending on your base OS.


### On Windows

> This is currently having a few issue

1. Download the zip file or clone this repository.
2. Navigate to the unzipped folder within the file browser.
3. Right-Click on `windows_install.bat` and select `Run as Administrator`
4. Test the installation by running the following from a command window in the directory of this project

   `mvn test  -Dsurefire.suiteXmlFiles=windows-only.xml`

#### Longer Instructions

1. The script should install Chocolatey the Windows package manager.
2. Install latest versions of 

    a. Firefox
    
    b. Chrome
    
    c. PhantomJS
    
3. Selenium drivers for the above and the Edgedriver

## Running Tests

The following commands are instructions on how to run the tests


### Intellij IDEA

There is a shared run configuration that has the maven target setup and another with a sample built in NUnit test runner option.

#### Safari Test

Safari requires the following steps to enable Selenium Webdriver tests to run:

1. Open Safari Preferences
2. Go to the Advanced Tab
3. Check the box at the bottom "Show Develop menu in menu bar"
4. Click on the Develop menu 
5. Click on "Allow Remote Execution"

Now Safari tests will work. 

If running tests only locally you can remove delete `//` from the  `@Test` line of the Safari class.
