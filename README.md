# Azure-VM-create

# Create an Azure Account and Deploy a Virtual Machine in the Cloud

![image](https://github.com/Afrocybersamurai/Azure-VM-create/assets/136266716/003eccc8-f363-4fe0-ad3d-9b0e5f007859)

Microsoft Azure is a cloud computing platform with numerous products and services. This guide will demonstrate how to create an account, utilize the portal, and create a virtual machine.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure
- Microsoft Remote Desktop (macOS) for virtual machines
- Windows Remote Desktop Connection

<h2>Configuration Steps</h2>

- Step 1: Create Azure Account
- Step 2: Azure portal and resource group
- Step 3: Create a virtual machine
- Step 4: Connect to virtual machine using Microsoft Remote Desktop on macOS

<h3>Step 1: Create Azure Account</h3>
First step is to create an Azure account. You can create an account with $200 of free credit for a month. 

<br>
<br>

Create an Azure account [here](https://azure.microsoft.com/en-us/free/).

![image](https://github.com/Afrocybersamurai/Azure-VM-create/assets/136266716/0df2137f-7cd1-419f-822d-0c4a1d1be2fe)


Follow all the prompts to create the account. 
You will need a credit card, which will not be charged until the $200 credit runs out or the account has been active for a month. 
Now that you have created your account, you are officailly a tenant in Azure.

<h3>Step 2: Azure portal and resource groups</h3>

With your newly created account, we can navigate to the Azure portal. 
The portal is where you can find all the products/resources and manage your subscriptions. 

The portal is located [here](https://www.portal.azure.com).

![image](https://github.com/Afrocybersamurai/Azure-VM-create/assets/136266716/f060b2ca-a490-4dc1-8059-fc2c97351adf)

In order to utilize some of the services in Azure, a resource group needs to be created. Resource groups store all resources that you are utilizing in Azure. This example will show how to deploy a Windows 10 virtual machine.

![image](https://github.com/Afrocybersamurai/Azure-VM-create/assets/136266716/f5623d81-07c3-4712-a669-e455edf73663)

When ready, click create resource groups. From there, you will need to name your resource group and select the region. The region will determine which Azure data center will be utilize. (US) West 3 was chosen for this example. 
Click "Review + Create" once finished

![image](https://github.com/Afrocybersamurai/Azure-VM-create/assets/136266716/1e34586d-9fee-46f9-a549-5fdbd56761c3)


<h3>Step 3: Create a virtual machine</h3>
Next we will create a virtual machine. At the portal, click on virtual machine and click create. 

![image](https://github.com/Afrocybersamurai/Azure-VM-create/assets/136266716/94f9e19d-4040-447e-8f32-02ef87abe47e)

![image](https://github.com/Afrocybersamurai/Azure-VM-create/assets/136266716/ce1c3c8f-2235-4bfc-8116-bf2eca4e8c78)

Once at the create virtual machine menu, follow all the instructions. Make sure to fill out all the areas in the red boxes (resource group, name, etc.). 
Don't worry about the other tabs such as disks and networking as they will be prefilled. 

![image](https://github.com/Afrocybersamurai/Azure-VM-create/assets/136266716/35a0bca9-4968-4fc3-8ff1-4f421ce73002)


Choose your size. I recommend an option with 2 vcpus or 4 vcpus (N.B you are allowed a max of 4vcpus at one time on the free accounts). Keep in mind the higher the specifications the faster the Virtual Machine and the more it costs to run.

![image](https://github.com/Afrocybersamurai/Azure-VM-create/assets/136266716/9eca4a1b-f669-438b-b566-7cfa64f547b4)

Input your name and password details. Keep this somewhere you will remember. 
Once this is all completed, your virtual machine will appear in your resource group. 


<h3>Step 4: Connect to virtual machine using Microsoft Remote Desktop (RDP)</h3>
The final step to this process is accessing the virtual machine using Microsoft Remote Desktop. 

# On MacOS
If you are a macOS user, you need to download the application in the App Store. 

<p align="center">
<img src="https://i.imgur.com/pp1yQTE.png" height="80%" width="80%" alt="Microsoft Remote Desktop"/>
</p>

In order to connect to the virtual machine, you will need the public IP address. You can find this on the right hand side of the following menu.

<p align="center">
<img src="https://i.imgur.com/gT6F62H.png" height="80%" width="80%" alt="SampleVM menu with arrow and circle"/>
</p>

Once Microsoft Remote Desktop is downloaded, open the application. Click add PC. Copy and paste the public IP address of the virtual machine that was created when prompted. Type in the username and password the click connect. 

<p align="center">
<img src="https://i.imgur.com/WcRdlX3.png" height="80%" width="80%" alt="Microsoft Remote Desktop 1"/>
</p>

<p align="center">
<img src="https://i.imgur.com/4IKJFik.png" height="80%" width="80%" alt="Windows 10 VM"/>
</p>

# On Windows

Navigate to the start button and type remoted desktop in the search bar.

![image](https://github.com/Afrocybersamurai/Azure-VM-create/assets/136266716/93dd8848-bc4e-41e3-acb3-b2ce2ebf2d3d)


![image](https://github.com/Afrocybersamurai/Azure-VM-create/assets/136266716/bb719d0c-5e9f-4600-b15b-ac2f61d11916)

Copy and paste the public IP address of the virtual machine that was created when prompted. Type in the username and password the click connect. 

Congratulations! You have created your first virtual machine within Azure. If you want to save your free $200 credits, make sure you delete ALL resource groups or stop your Virtual machine when not in use, because you will continue to be charged for their use.



