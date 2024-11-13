# Exercise-8-Basic-Web-Automation---Fill-a-Web-Form

## Aim:
To automate the process of filling out a web form using the Application/Browser activity in UiPath Studio.

## Equipment Required:
UiPath Studio installed on your computer.<br>
Web Browser (e.g., Chrome, Edge, with UiPath extensions installed).<br>
Computer with:<br>
Minimum 4 GB RAM.<br>
Minimum 2.0 GHz CPU.<br>
Windows operating system.<br>
A Web Form to be automated.

## Procedure:
### Create a New Project in UiPath Studio:
Open UiPath Studio and create a new project by selecting Process under the New Project tab.<br>
Name the process (e.g., Web Form Automation Using Application/Browser) and click Create.

### Install the Browser Extension:

To interact with a web browser, install the necessary UiPath browser extension:<br>
Go to the Tools section in UiPath Studio.<br>
Install the extension for the browser you will use (e.g., Chrome or Edge).

### Use Application/Browser Activity:

Instead of using the Open Browser activity, we will use the Use Application/Browser activity.<br>
In the Activities panel, search for Use Application/Browser and drag it into the Main sequence.<br>
In the Application/Browser field, click Indicate Application on Screen, then navigate to the browser where the web form is located and indicate the web form window or tab.<br>
Once the browser is selected, it will embed the browser as part of the automation.

### Navigate to Web Form:

After setting up the Use Application/Browser activity, use the Navigate To activity to navigate to the web form’s URL.<br>
Inside the Use Application/Browser container, search for Navigate To and add it to the workflow.<br>
In the URL property of Navigate To, enter the URL of the web form.

### Fill in Web Form Fields:

To input data into the form, use Type Into activities for each field on the form.<br>
Steps:<br>

Search for the Type Into activity in the Activities panel and drag it into the sequence under the Navigate To activity.<br>
Click the Indicate on Screen button in the Type Into activity and select the form field where you want to enter the data (e.g., the Name field).<br>
Enter the text (e.g., "John Doe") in the Text property of the Type Into activity.<br>
Repeat this step for each form field, such as Name, Email, Phone, etc.

### Select Dropdowns or Checkboxes (if applicable):

For dropdown fields, use the Select Item activity.<br>
For checkboxes or radio buttons, use the Check activity.<br>
Steps:<br>
Search for Select Item for dropdowns. Indicate the dropdown field and specify the value in the Item property.<br>
Use Check to select checkboxes or radio buttons, and indicate the field on the web form.

### Submit the Form:

To submit the form, use the Click activity.<br>
Drag the Click activity below the fields that you filled out.<br>
Click Indicate on Screen in the Click activity and select the Submit button on the web form.

### Save and Run the Workflow:

Press CTRL+S to save the workflow.<br>
Click the Run button to execute the automation.<br>
The robot will open the web form in the browser, fill in the details as provided in the Type Into activities, and submit the form.

## UiPath WorkFlow:
![image](https://github.com/user-attachments/assets/280f307b-4b63-4690-937e-ded19b22d7f7)
![image](https://github.com/user-attachments/assets/3a11150f-9afb-433d-90b6-f45c2b91aff1)
![image](https://github.com/user-attachments/assets/1123cd1e-41fa-4e60-8fcb-34216d73ed61)
![image](https://github.com/user-attachments/assets/55d2cf64-5050-4ecf-99d6-30338380da8b)
![image](https://github.com/user-attachments/assets/cf7d5448-4720-43c9-a7c0-68f25b49124a)
![image](https://github.com/user-attachments/assets/30380f6e-ebb6-4917-aaa9-93c2edf4493d)
![image](https://github.com/user-attachments/assets/0bccfe07-3676-40d4-8011-c8a14f36ed35)
![image](https://github.com/user-attachments/assets/a741ec06-bbbf-44ac-981d-93c9f327ac2b)
![image](https://github.com/user-attachments/assets/66bd1307-dbfd-49b2-bebd-79bb1b3a7696)

## Result:
The web form is successfully filled and submitted using UiPath Studio with the Application/Browser activity, demonstrating the automation of a web-based form without explicitly opening a browser each time.
