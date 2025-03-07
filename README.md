<p align="center">
<img src="https://github.com/user-attachments/assets/0c9a5058-f465-477c-be11-3de15009f17b" height="350" width="350"
</p>

<h1>Installing osTicket</h1>
This tutorial outlines the steps to install osTicket to a Windows 10 virtual machine.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- osTicket system
- Internet Information Services (IIS)
- PHP 7.3.8
- PHP manager for IIs
- Rewrite module
- MySQL
- Visual C++

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)


<h2>Installation Steps</h2>

<p>
Retrieve the public IP address of the newly created virtual machine to connect via remote desktop. <br /> <br />
<img src="https://github.com/user-attachments/assets/d180b1c5-ad12-45bc-ae5c-2e0fc6895c2c" height="80%" width="80%"/>
</p>
<br />


<p>
Download osTicket installation zip file and unzip the folder. <br /> <br />
<img src="https://github.com/user-attachments/assets/9f6b0518-1811-4e7b-ba2c-c01dcaf9dc42" height="80%" width="80%"/>
</p>
<br />



<p>
Navigate to Windows features and turn on CGI under internet information services>application development features dropdown menus. <br /> <br />
<img src="https://github.com/user-attachments/assets/2f463296-64c4-452e-981f-0b85263fa6a6" height="80%" width="80%"/>
</p>
<br />


<p>
Install PHP manager for IIS. <br /> <br />
<img src="https://github.com/user-attachments/assets/53bb1463-b491-4dcd-a5e2-bd259d2288d4" height="80%" width="80%"/>
</p>
<br />



<p>
Install rewrite module. <br /> <br />
<img src="https://github.com/user-attachments/assets/93d049d6-08fa-4ee9-a492-98b7a704d937" height="80%" width="80%"/>
</p>
<br />


<p>
Create a directory on the C drive and name it PHP. <br /> <br />
<img src="https://github.com/user-attachments/assets/37fd5f61-b237-418e-bc74-fcca6ad9fd8c" height="80%" width="80%"/>
</p>
<br />




<p>
Extract PHP 7.3.8 to the folder we previously created in order to install the PHP language binaries. <br /> <br />
<img src="https://github.com/user-attachments/assets/d28ac334-3cec-4424-8a43-9ee6441164ee" height="80%" width="80%"/>
</p>
<br />



<p>
Install Visual C++ redistributable (x86) package. <br /> <br />
<img src="https://github.com/user-attachments/assets/5bb51aa5-605c-4a4f-b5a4-8ae0674c7deb" height="80%" width="80%"/>
</p>
<br />




<p>
Install MySQL (osTicket uses this to store data). <br /> <br />
<img src="https://github.com/user-attachments/assets/23be52d4-ba2a-4458-a0e3-4118379dd2c6" height="80%" width="80%"/>
</p>
<br />



<p>
Choose the standard configuration while installing MySQL. <br /> <br />
<img src="https://github.com/user-attachments/assets/3d730a48-7ace-4160-adf1-b125476d55ac" height="80%" width="80%"/>
</p>
<br />



<p>
Open IIS as an admin. <br /> <br />
<img src="https://github.com/user-attachments/assets/c6e0563c-a1ba-4379-a272-305a45ab75c5" height="80%" width="80%"/>
</p>
<br />




<p>
Register PHP from within IIS. <br /> <br />
<img src="https://github.com/user-attachments/assets/f6558a7a-71de-4935-a056-471bca0cf011" height="80%" width="80%"/>
</p>
<br />



<p>
After double-clicking on PHP manager from within IIS, click "Register new PHP version", browse to previously created PHP folder, and select php-cgi application. <br /> <br />
<img src="https://github.com/user-attachments/assets/d7a1eb20-65eb-4b36-90db-110952fa86c1" height="80%" width="80%"/>
</p>
<br />



<p>
Stop, then start webserver. <br /> <br />
<img src="https://github.com/user-attachments/assets/a777972f-cb4e-4d7a-a21b-a1c6f2782461" height="80%" width="80%"/>
</p>
<br />





<p>
Extract the osTicket zip file. <br /> <br />
<img src="https://github.com/user-attachments/assets/3df2e6f5-075b-4918-9123-07e4e3034c38" height="80%" width="80%"/>
</p>
<br />



<p>
Copy the upload folder into C:\inetpub\wwwroot and rename it to osTicket. <br /> <br />
<img src="https://github.com/user-attachments/assets/80f1f3b8-d95b-414e-8c73-daf814446f25" height="80%" width="80%"/>
</p>
<br />




<p>
After stopping and starting the server, navigate to Sites>Default Web Site>osTicket and click on "Browse" on the right side of the screen. <br /> <br />
<img src="https://github.com/user-attachments/assets/a9b5d718-3598-4fad-a9c1-febb6a391715" height="80%" width="80%"/>
</p>
<br />



<p>
At this point, the osTicket installer should open up. <br /> <br />
<img src="https://github.com/user-attachments/assets/6b0e9b22-21eb-4a5f-91bd-5f909655bf4e" height="80%" width="80%"/>
</p>
<br />




<p>
Open PHP manager under osTicket subfolder and enable PHP extension. <br /> <br />
<img src="https://github.com/user-attachments/assets/a1ca5808-7057-4cfd-b708-52f676538ab7" height="80%" width="80%"/> <br /> <br />
<img src="https://github.com/user-attachments/assets/893ebb14-f7f3-4c49-8b56-2f4268e64119" height="80%" width="80%"/> <br /> <br />
</p>
<br />


<p>
Enable php_imap.dll, php_intl.dll, and php_opcache.dll. <br /> <br />
<img src="https://github.com/user-attachments/assets/233d4e77-ff42-4530-ac33-356465c8beae" height="80%" width="80%"/>
</p>
<br />




<p>
Navigate to C:\inetpub\wwwroot\osTicket\include and rename the ost-sampleconfig.php file to ost-config.php. <br /> <br />
<img src="https://github.com/user-attachments/assets/4a43aad9-1ea6-43f8-9488-f33f1d918048" height="80%" width="80%"/> <br /> <br />
<img src="https://github.com/user-attachments/assets/f8424263-c358-4211-a592-2d42a0778a13" height="80%" width="80%"/> <br /> <br />
</p>
<br />




<p>
Right-click on the properties of the ost-config.php file, go to the security tab, click advanced, and click disable inheritance to remove all inherited permissions. <br /> <br />
<img src="https://github.com/user-attachments/assets/ae65ba79-35a8-4c34-ba0d-94e8cf1ad441" height="80%" width="80%"/>
</p>
<br />



<p>
After removing all inherited permissions, let's add new permissions. Click on "select a principal" and type Everyone in the box just for this exercise since we don't know what user osTicket will represent. We will give the user full control. Now osTicket has full permissions over the configuration file. <br /> <br />
<img src="https://github.com/user-attachments/assets/9406c331-1d6f-4589-8ee6-8ae5b36ccd1e" height="80%" width="80%"/>
</p>
<br />



<p>
Continue filling out the top portion of the osTicket basic installation form. <br /> <br />
<img src="https://github.com/user-attachments/assets/6a2899b0-608b-4c40-804c-71fffe740582" height="80%" width="80%"/>
</p>
<br />



<p>
Navigate to osTicket-Installation-Files installation folder and install HeidiSQL, which allows us to connect and configure the database. <br /> <br />
<img src="https://github.com/user-attachments/assets/b11d00a4-173f-491e-867e-91a3464dcbef" height="80%" width="80%"/>
</p>
<br />




<p>
We will use HeidiSQ to make a connection to our database and set up a database for osTicket to use; then, we can use this information to fill out the bottom of the basic installation form. <br /> <br />
<img src="https://github.com/user-attachments/assets/b11d00a4-173f-491e-867e-91a3464dcbef" height="80%" width="80%"/>
</p>
<br />


<p>
Click new SQL, type in username and password credentials, and click open to create a new session. <br /> <br />
<img src="https://github.com/user-attachments/assets/fc878c2a-df65-43c7-aef3-6947a2502984" height="80%" width="80%"/>
</p>
<br />



<p>
Create a new database named osTicket in HeidiSQL. <br /> <br />
<img src="https://github.com/user-attachments/assets/5ab82e23-fafd-49cc-b6cc-3af5d34704af" height="80%" width="80%"/>
</p>
<br />



<p>
The osTicket database in HeidiSQL has been created. <br /> <br />
<img src="https://github.com/user-attachments/assets/2a9bd714-03ea-4955-9969-84016dce02f3" height="80%" width="80%"/>
</p>
<br />




<p>
With the osTicket HeidiSQL server created, we can complete the database settings part of the form in the browser. <br /> <br />
<img src="https://github.com/user-attachments/assets/f1085e90-2be8-4388-8dc9-6690be3ddcf1" height="80%" width="80%"/>
</p>
<br />



<p>
osTicket has been installed! <br /> <br />
<img src="https://github.com/user-attachments/assets/5d772942-ff5f-4452-a9e7-2ba331b88600" height="80%" width="80%"/>
</p>
<br />




