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
- rewrite module
- MySQL
- Visual C++

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)


<h2>Installation Steps</h2>

<p>
<img src="https://github.com/user-attachments/assets/d180b1c5-ad12-45bc-ae5c-2e0fc6895c2c"</p>
<p>Retrieve public IP address of newly created virtual machine to connect via remote desktop</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/9f6b0518-1811-4e7b-ba2c-c01dcaf9dc42"</p>

<p>download osTicket installation zip file and unzip folder</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/2f463296-64c4-452e-981f-0b85263fa6a6"</p>

<p>navigate to windows features and turn on CGI under internet information services>application development features dropdown menus</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/53bb1463-b491-4dcd-a5e2-bd259d2288d4"</p>

<p>Install PHP manager for IIS</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/93d049d6-08fa-4ee9-a492-98b7a704d937"</p>

<p>Install rewrite module</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/37fd5f61-b237-418e-bc74-fcca6ad9fd8c"</p>

<p>Create directory on C drive and name it PHP</p>
<br />




<p>
<img src="https://github.com/user-attachments/assets/d28ac334-3cec-4424-8a43-9ee6441164ee"</p>

<p>Extract PHP 7.3.8 to folder we previously created in order to install the PHP language binaries</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/5bb51aa5-605c-4a4f-b5a4-8ae0674c7deb"</p>

<p>Install Visual C++ redistributable (x86) package</p>
<br />




<p>
<img src="https://github.com/user-attachments/assets/23be52d4-ba2a-4458-a0e3-4118379dd2c6"</p>

<p>Install MySQL (osTicket uses this to store data)</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/3d730a48-7ace-4160-adf1-b125476d55ac"</p> 

<p>Choose standard configuration while installing MySQL</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/c6e0563c-a1ba-4379-a272-305a45ab75c5"</p>

<p>Open IIS as an admin</p>
<br />




<p>
<img src="https://github.com/user-attachments/assets/f6558a7a-71de-4935-a056-471bca0cf011"</p>

<p>Register PHP from within IIS</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/d7a1eb20-65eb-4b36-90db-110952fa86c1"</p>

<p>After double-clicking on PHP manager from within IIS, click "Register new PHP version", browse to previously created PHP folder, and select php-cgi application</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/a777972f-cb4e-4d7a-a21b-a1c6f2782461"</p>

<p>Stop, then start webserver</p>
<br />





<p>
<img src="https://github.com/user-attachments/assets/3df2e6f5-075b-4918-9123-07e4e3034c38"</p>

<p>Extract osTicket zip file</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/80f1f3b8-d95b-414e-8c73-daf814446f25"</p>

<p>copy upload folder into C:\inetpub\wwwroot and rename to osTicket</p>
<br />




<p>
<img src="https://github.com/user-attachments/assets/a9b5d718-3598-4fad-a9c1-febb6a391715"</p>

<p>After stopping and starting server navigate to Sites>Default Web Site>osTicket and click on "Browse" on the right side of the screen</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/6b0e9b22-21eb-4a5f-91bd-5f909655bf4e"</p>

<p>At this point the osTicket installer should open up</p>
<br />




<p>
<img src="https://github.com/user-attachments/assets/a1ca5808-7057-4cfd-b708-52f676538ab7"</p>
<img src="https://github.com/user-attachments/assets/893ebb14-f7f3-4c49-8b56-2f4268e64119"</p>

<p>Open PHP manager under osTicket subfolder and enable PHP extension</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/233d4e77-ff42-4530-ac33-356465c8beae"</p>

<p>Enable php_imap.dll, php_intl.dll, and php_opcache.dll</p>
<br />




<p>
<img src="https://github.com/user-attachments/assets/4a43aad9-1ea6-43f8-9488-f33f1d918048"</p>
<img src="https://github.com/user-attachments/assets/f8424263-c358-4211-a592-2d42a0778a13"</p>
  
<p>Navigate to C:\inetpub\wwwroot\osTicket\include and rename ost-sampleconfig.php file to ost-config.php</p>
<br />








