# Sencha Touch setup (Version 2.0.2 - Windows)

## Sencha Touch 
 Sencha Touch is HTML5 mobile application framework. We can say Sencha Touch is use to create Hybrid mobile application means code once and create application for all the mobile platform(iOS , Android , Blackberry, Windows).

## Step1 - Required Software

To work with Sencha Touch we need following software:

1. Sencha Touch SDK( Version-  2.2.1)  - download and unzip it to any directory
	Downlad it from here - (http://www.sencha.com/products/touch/)

2. Sencha Cmd( Version- Cmd 4.0.1.45) - download it from following link and install it. To check correctly installed or not . open command promt and type sencha it will display version 
  Downlad it from here (http://www.sencha.com/products/sencha-cmd/download) and install it.

2. XAMPP (Apache Web Server) or we can use apache software (Optional)
   Downlad it from here (https://www.apachefriends.org/download.html) and installed it.

3. Sencha supports only Chrome , Safari or IE10+ browser and for mobile you can use Chrome , Safari  , IE10+.
   
4. JRE (Java Run Time Environment)- As Sencha Cmd written in  Java and needs the JRE to run
   Downlad it from here  (http://www.oracle.com/technetwork/java/javase/downloads/jre7-downloads-1880261.html) and install it.

5. Ruby(version 1.9.3p545 ) - Ruby use to install require gem files(compiled CSS used by sencha). 
   install compass 0.12.6 



## Step2 - Creating project 

1. Create a new directory named as myApp(You can give any name), and paste the extract Sencha Touch folder into myApp folder.
   e.g - Suppose I create directory as in D:\myApp , copy sencha-touch-2.1.0 and paste in myApp.
   so it is in D:\myApp\sencha-touch-2.1.0 

2. Open command prompt > go to myApp sencha-touch folder > cd D:\myApp\sencha-touch-2.1.0
   D:\myApp\sencha-touch-2.1.0>

   use following command to create sencha project skeletone structure
   D:\myApp\sencha-touch-2.1.0>sencha -sdk D:\myApp\touch-2.2.1 generate app MyFirstApp D:\myApp

   Here, 
     1. D:\myApp\touch-2.2.1 - Path of Sencha Touch SDK
     2. MyFirstApp - is the name of our app.
     3. D:\myApp - It is the directory where you want all project specific files to be genereated.
     (If you dont specify D:\myApp , it will create peoject in current directory from where you are running generate command )

3. After successfully installation , this command creates project skeleton in myApp directory.

4. Create Virtual Host by any name say local.sencha.com to access the pages.

## project directory structure 
   - .sencha
   - app : all controller , model , store , util , view are store in this folder.
   - build 
   - packages
   - resources - all css , images goes to this folder.
   - touch
   - touch-2.2.1
   - app.js : Main entry point of app.
   - app.json : configuration file for application where we can instruct application and sencha command to use , create or update in certainer resource.
   - bootstrap.js
   - bootstrap.json
   - build.xml
   - index.html : Tha main HTML file of application
   - packager.json : configuration file used by Sencha command for native packaging.

### for more details information of sencha use Sencha Doc
	(http://docs.sencha.com/touch/2.0.2/#!/api)


