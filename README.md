<p align="center">
<img src="https://github.com/user-attachments/assets/0c9a5058-f465-477c-be11-3de15009f17b" height="350" width="350"
</p>

<h1>Install osTicket</h1>
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
<img src="https://github.com/user-attachments/assets/d180b1c5-ad12-45bc-ae5c-2e0fc6895c2c" height="200%" width="200%"</p>
<p>Retrieve public IP address of newly created virtual machine to connect via remote desktop</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/9f6b0518-1811-4e7b-ba2c-c01dcaf9dc42" height="200%" width="200%"</p>

<p>download osTicket installation zip file and unzip folder</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/2f463296-64c4-452e-981f-0b85263fa6a6" height="200%" width="200%"</p>

<p>navigate to windows features and turn on CGI under internet information services>application development features dropdown menus</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/53bb1463-b491-4dcd-a5e2-bd259d2288d4" height="200%" width="200%"</p>

<p>Install PHP manager for IIS</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/93d049d6-08fa-4ee9-a492-98b7a704d937" height="200%" width="200%"</p>

<p>Install rewrite module</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/37fd5f61-b237-418e-bc74-fcca6ad9fd8c" height="200%" width="200%"</p>

<p>Create directory on C drive and name it PHP</p>
<br />




<p>
<img src="https://github.com/user-attachments/assets/d28ac334-3cec-4424-8a43-9ee6441164ee" height="200%" width="200%"</p>

<p>Extract PHP 7.3.8 to folder we previously created in order to install the PHP language binaries</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/5bb51aa5-605c-4a4f-b5a4-8ae0674c7deb" height="200%" width="200%"</p>

<p>Install Visual C++ redistributable (x86) package</p>
<br />




<p>
<img src="https://github.com/user-attachments/assets/23be52d4-ba2a-4458-a0e3-4118379dd2c6" height="200%" width="200%"</p>

<p>Install MySQL (osTicket uses this to store data)</p>
<br />



<p>
<img src="https://github.com/user-attachments/assets/3d730a48-7ace-4160-adf1-b125476d55ac"200%" width="200%"</p>

<p>Choose standard configuration while installing MySQL</p>
<br />




























