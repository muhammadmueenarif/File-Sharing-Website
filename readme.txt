File sharing websites are special type of website developed to store files. file can be multimedia, images, audios, 
videos, and any other files like texts or pdf or any applications or software, apk or exe files. 

when files stored, user can share files on internet. Popular files sharing websites are google drive, dropbox, 
microsoft one drive, box, mega, mediafire. 

Requirements for website? Web hosting (hosting should have more space so it can store more files), 
Domain (domain to access website. you can use any domain), and last is file sharing software or script. we
will use project send as software or script. 

Project send is free and open source software to upload files and then share files. it is self hosted application
means we can install it on our own VPS or web hosting. 
it is free secure and user friendly. Download it from official website of https://projectsend.org.


Uploading project send to web hosting.

I am using free web hosting to host a file sharing website but you should use premium if you want to run 
proper project. ( bythost and many other sites available)
https://cpanel.byethost.com. after opening c panel of web hosting, go to file manager and open domain name folder, then open htdocs folder. 
here paste the project send zip file that we Downloaded. 
Alternatively, we can upload projectsend using ftp. but for this, we need ftp account details. ftp account details are
generally available in your web hosting cpanel. 


How to install projectsend? 
open the url where we uploaded our projectsend. (open your website domain in browser).
Project installation option will be shown. it will ask to set database configuration. we will enter out details 
and also customize the maximum upload file size which is 2gb by default. other information related to website configuration 
will be showing.

we can set website database using php my admin. goto cpanel and mysql database option. enter name of database and click on create.
database will be created with all details. copy these details and goto projectsend installation page. enter host name, 
copy database name, username and enter on projectsend page. then enter password. after entering details and verify, 
goto write config file. our config file is written successfully. now click on continue to installation. 

enter your details like website name, your name, email, and login password etc., then click on install and projectsend is installed
successfully. now just enter home page and enter login username and password. 


Once installed, 
enter your website domain name (like abc.com) in browser and enter login details and enter. we will see information of our web hosting here. 
we can manage and create files and categories. we can add client, manage client groups from left side option.
in system users, we can manage users like admin and other if we add more users. in templates, we can check but default is good. 
in email template section, we can manage emails. in tools option, we can check action log and test email configuration in our website. 
(https://domain_name/dashboard.php) (replace domain name with your domain name).


How to change logo? 
login in website, then goto options menu and click branding, choose logo and save it. 


Change footer and timezone? 
goto option, click on general option. there will be option of use custom footer text, enable it and enter text. 
in general option, we can change website name and timezone also. and click save. write &copy: if you want to show 
copyright symbol in the footer. 


What files extension allowed to upload? how to add more files extension?
click on options, and goto security section. here we will see allowed extension and we can add more if we want. 


Allow users to create account on website?
now if we goto login page, it shows new users are not allowed to create account and they need to contact admin if they want to create account.
goto options, click on clients, there is option for new registration. enable client can register themseleves and also use auto approve if you want. 
also option that client can upload and delete their files. save it and now other users can register. 
Goto admin option and click on security and enable captcha option to avoid spamming. enable this icon. 
then search google recaptcha on browser (make sure you are login with your google account). and open https://google.com/recaptcha/about. click on v3 admin console. 
click on + icon to add new website. enter label to identify website. there are 2 options for recaptcha. click on v2. 
and then select i am not a robot checkbox. enter domain name and accept terms and submit details. 
it will show site key and secret key. copy site key and paste it in your website where you are logged in and paste it in related box. 
similarly add secret key box. 


Add user manually?
goto clients option and click on add new. fill the details and submit. 

manage clients?
click on clients and then click manage clients. perform the desired action. 

How to add system users?
goto system users option and click add new. fill details and submit. we can create one of three sytem user. 
first is system administrator with full access, other is account manager and last is uploader only. click on add user. 

if want to manage system users, then just click on manage system users in sidebar. 


How to create category?
goto file and click on categories. then enter name of cateogory, add description and click create. similarly we can add categories as we want. 

How to upload file?
Goto file option in side. click on upload. select file and then check other details like if you want to delete the files after some certain time period then you can use that option. 
file will expire on that day. select the category in which we want to upload. allow public Download. and save. 
to get the Download link of the file, click on public button and click on url and link will be copied from where anyone can Download.


goto files, click on manage files. we can edit our files and their details whenever we want. 


Adding advertisement? How to show ads on Download page of website?
open cpanel. and open file manager. open htdocs and find Download.php file. we need to edit this file. 
find the code <?php if ($can_download == true) { ?>}

add your p tag above this and add text that you want to show. 

next is banner ads. just copy your banner source and use img tag instead of p tag and it will show banner ads instead of text ads. 
use a or link tag with image if we want to open any other url on the click of the image. 
we can show adsence or any other ads in this way. 

