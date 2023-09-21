
# Azure Function

We have the necessity of running our python script manually every time, to do certain task (or) to get the required output based on regular basics

So Azure Function helps us to automate the python script




### Logo:

![Logo](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/Azure.png)


## Documentation

Refer this link for detailed explaination👇 \
\
https://learn.microsoft.com/en-us/azure/azure-functions/functions-develop-vs-code?tabs=node-v3%2Cpython-v2%2Cin-process&pivots=programming-language-python


## Local Testing:
Before we deploy our python code in AZURE, we need to check the behaviour of the python script in local with the help of visual studio code(IDE).
## Download Link
Install the Azure Functions Core Tools(Only for running it locally) \
\
Click the link below to download the azure function core tool(Recommended for 64 bit) 👇 

https://go.microsoft.com/fwlink/?linkid=2174087

## Steps for setup
### step 1:
Create a Function app in azure with Globally unique name 

Refer this documentation link to create a Function app 👇 \
https://learn.microsoft.com/en-us/azure/azure-functions/functions-create-scheduled-function\
\
The created function app name will be displayed after sign in(step: 04) from visual studio code \
E.g: XYZDataLoad
### step 2:
Go to Visual studio code and install these 4 extensions are: \
👉 Azure Account \
👉 Azure Resources \
👉 Azure Functions \
👉 Azurite

![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/Screenshot%202023-09-20%20193448.png)

![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/Azurite.png)

After Installing all these you will see the Azure icon on the left side of Visual Studio code like this 👇
 
![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/azuree.png)

### step 3:
Click the Azure icon and again click sign in to Azure and it will make a connection between azure and visual studio code

![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/sign.png)

### step 4:
After Sign-in you can see the function app you created in (step 1) with in visual studio code
![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/Azure_function_app.png)


### step 5:
Create a new project in workspace
![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/step_1_Create_new_project.png)


### step 6:
Select Python (Programming module V2)
![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/v2.png)

### step 7:
Select a virtual envirement that you want to use
![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/select_environment.png)

### step 8:
Select time trigger, Since we are going to trigger the python script irrespective with time
![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/step_4_time_trigger.png)

### step 9:
We should name the function that we want to create
![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/step_5_name_for_time_trigger.png)

### step 10:
Setting up the cron expression to run the python script for every 5 minutes automatically
![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/step_6_setting_cron_for_every_5_min.png)


### step 11:
Finally it will create a new project

![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/step_7_settup_project.png)


And it will automatically bring the default(supporting files) inside the virtual envirement that we created, which is below👇 \
👉 function_app.py \
👉 getting_started.md \
👉 host.json \
👉 local.settings.json \
👉 Requirement.txt 

![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/auto_genereted_file.png)

### step 12(IMPORTANT STEP):

![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/func.png)

In function_app, By Default it will have 10 lines of code 

👉Paste your python script inside function_app.py \
👉don't rename the function_app.py name, Since it is pre-defined
    
### step 13:
✍️Write the supporting libraries in the Requirement.txt \
E.g: I am using library like pandas, sqlalchemy, requests, azure-functions and pyodbc, So i wrote all them in line by line on Requirement.txt \
\
![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/requirement.png)

### step 14:
#### Installation
👉 Installing the required libraries that is only needed

pip install azure-functions \
pip install sqlalchemy \
pip install requests \
pip install pandas \
pip install pyodbc
    
### step 15:
#### Run Function
Before Running the function, check whether the virtual Envirement is active\
\
 👉Use a shortcut key to start the func app --> fn + F5 \
 (or) \
 👉Open a new terminal and run using --> func start

At last, the program will run at a predefined time interval that we establish.
## Function Output

If our program is correct, it used to give us a output like this 👇 

![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/output.png) 

👉Work process started and initiated \
👉Executing 'Function.(Our function name)' \
👉Python timer trigger function ran at yyyy-mm-dd hh-mm-ss sssuuu

If incase the program is not running we need to check with the step 12 👈 again
## Deployment
If the function is running good in local, Then click deploy to Function App...
![App Screenshot](https://raw.githubusercontent.com/GowthamK66/Newell/main/readme.so/Final_deploy.png)



## Used By

This Azure Function App is used by the following companies:

- Walmart
- Target
- Newell


## Support

For support🤝, \
contact via Teams (or) email👇 \
mithun.mohan@newellco.com or \
chinnathambi.murugesan@newellco.com or \
gowtham.kalidass@newellco.com 

## Authors

- [@Gowtham.kalidass](https://github.com/GowthamK66)


