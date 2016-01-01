# Facebook Marketing Automation Java Application
The aim of this application is to provide easy &amp; extensible interface to automate facebook marketing including creating custom audience, creating facebook campaigns. 

FMA (Facebook Marketing Automation) main objective is to become bridge between CRM & facebook. FMA will act as zero work for any business having CRM which want to utilize Facebook's custom audience and campaign management solution. 

FMA is based on flexible File & Database source for creating Facebook custom audience. FMA is highly configurable for taking CRM data from definable data directory. It will process the file(s) and create custom audience. You can also provide some meta data about custom audience. 

FMA also have fully capability of creating and managing Facebook campaigns using open interface File/Database where campaign information are provided as XML file. 

FMA is Java based web app which requires apache tomcat 7+ and totally independent which application can use FMA for creating custom audience and managing facebook campaing. 

#Initial Setup
1. Crate a facebook application at http://developers.facebook.com/apps, lets say its name is FMA APP
2. Create/Setup your facebook ads account and get ads account id 
3. You need valid/live ACCESS TOKEN, use https://developers.facebook.com/tools/explorer/ to generate ACCESS TOKEN for FMA APP with ads_management permission
4. By default facebook access is short lived approximately for 2 minutes, you can extend ACCESS TOKEN for 60 days for better application working at https://developers.facebook.com/tools/accesstoken/
4. Provide app_id & app_secret

#Getting Started
1. Now you have all facebook related configuration. Let's put update some of application configuration. 
2. Open /FMA App/resources/application.properties and modify the following information
    appid=test
    secert=
    access_token=
    act_ad=
    crm_data=/home/data
3. Now you are all setup to run FMA. For testing, just place phone/email based file at /home/data. FMA will be monitoring crm_data configurated location continously and when any file is created/copyied into this location it will automatically pick this CRM file and will create custom audience. 
4. File formats for custom audience and campaing creation will be documented very soon. 

#Furture Work
