# Google_Form_Automate
Automate google Form :

Step1 : Launch the google form using url and use driver.get method
	URL:"https://docs.google.com/forms/d/e/1FAIpQLSep9LTMntH5YqIXa5nkiPKSs283kdwitBBhXWyZdAS-e4CxBQ/viewform" 
Step2 : Go to name field locate xpath for name field and enter data as "Crio Learner" use driver.send() method
	xpath:"(//input[@type="text"])[1]"
Step3 : Go to next text fiel Why are you practicing Automation? and enter text as "I want to be the best QA Engineer! epochtime"
	create epoch time java programme in wrapper.java file and make a call here
	xpath:""
Step4 :Go to radio btn and use for loop to travel from diffenrent radio btn to selected needed one use common xpath 
	xpath: ""


Automate Google Form
Step 1: Launch the Google Form
	- Open the Google Form using Selenium WebDriver.  
	-Use `driver.get() method.  
  URL:"https://docs.google.com/forms/d/e/1FAIpQLSep9LTMntH5YqIXa5nkiPKSs283kdwitBBhXWyZdAS-e4CxBQ/viewform"    

Step 2: Enter Name  
- Locate the Name input field using XPath.  
- Enter the text "Crio Learner" using `sendKeys()` method.  
- XPath:(//input[@type="text"])[1]  

Step 3: Enter Text in "Why are you practicing Automation?"  
- Locate the text area and enter "I want to be the best QA Engineer!" along with an epoch timestamp.  
- Call the `getEpochTimeAsString()` function from `Wrappers.java`.  
- XPath://textarea[contains(@class,'KHxj8b')]  

Step 4: Select a Radio Button  
- Use a for loop to iterate through different radio buttons.  
- Select the required radio button dynamically.  
- XPath://div[@role='radio']  

Step 5: Select Checkboxes  
- Locate checkboxes using XPath and click on them.  
- Example checkboxes: **Java, Selenium, TestNG.  
- XPath://span[contains(@class,'n5vBHf') and contains(text(),'Java')]/../../preceding-sibling::div[contains(@id,'i')]  

Step 6: Select an Option from Dropdown
- Locate and click on the dropdown.  
- Use `Wrappers.dropDownClick(driver, "Mr")` to select the value "Mr".  
- XPath://div[contains(@class,'QXL7Te')]//span[text()='Mr']  

Step 7: Enter Date (7 Days Ago) 
- Get the date 7 days ago using `Wrappers.getdateSevenDaysAgo()`.  
- Enter the value in the date field.  
- XPath://input[@type="date"] 

Step 8: Enter Time and Submit  
- Locate Hour and Minute fields and enter `07:30`.  
- Click the Submit button.  
- XPaths:  
  - Hour://input[@aria-label="Hour"]  
  - Minute://input[@aria-label="Minute"]  
  - Submit Button://span[text()="Submit"]
