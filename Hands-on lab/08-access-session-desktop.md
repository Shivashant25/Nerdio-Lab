# Lab 8: Access the Desktop using AVD Desktop Client

## Overview

Azure Virtual Desktop (AVD) integrates virtual desktop infrastructure (VDI) and the cloud. AVD is Microsoft Azure’s platform-as-a-service (PaaS) offering from Microsoft. It enables small to large cloud consumers to provide remote applications and full desktops from Microsoft cloud to their end-users. Azure Files is also a  platform service (PaaS) and is one of the recommended solutions for hosting FSLogix containers for AVD users. In this lab, you'll be accessing the Desktop using the AVD Desktop Client and verifying the User profiles stored in the File share

## Exercise 1: Access the Desktop using AVD Desktop Client

In this exercise, we will access the Desktop and RemoteApps assigned to us in the previous exercise using the AVD Desktop client.

>#### **Note:** You have to perform this exercise in **Your Own PC/computer/workstation.** Do not perform this exercise within the JumpVM.

1. From the JumpVM, Go to **Start** and search for **Remote desktop** and open the remote desktop application with the exact icon as shown below.

   ![ws name.](media/4s7.png)
   
1. Once the application opens, click on **Subscribe**.

   ![ws name.](media/4s8.png)
  
1. Enter your **credentials** to access the workspace.

   - Username: *Paste your username* **<inject key="Nmm User 01" />** *and then click on **Next**.*
   
   ![ws name.](media/4s9.1.png)

   - Password: Paste the password of ***nmmuser01*** which you had copied earlier *and click on **Sign in**.*

   ![ws name.](media/410.1.png)
   
   >**Note:** If there's a popup entitled **Help us protect your account** click **Skip for now (14 days until this is required)**

   ![](media/4s11.png)

   Make sure to **uncheck** *Allow my organization to manage my device* and click on **No, sign in to this app only**.

   ![ws name.](media/4s12.png)
   
1. The AVD dashboard will launch, then double click on the **Session Desktop** to access it.

    ![ws name.](media/4s13.png)
    
1. A window saying *Starting your app*, will appear. Wait for a few seconds, then enter the password of ***nmmuser01*** which you had copied earlier, and click on **OK**.
   
    ![ws name.](media/4s14.1.png)
    
1. Wait for the Session Desktop to connect.

    ![ws name.](media/4s15.png)
    
1. Your virtual desktop will launch and look similar to the screenshot below. You can exit from the window by clicking on **X *i.e., the close button***. 
        
    ![ws name.](media/4s16.png)
   
## Exercise 2: Verifying the User profiles stored in the File share

In this exercise, you'll be verifying the user profiles stored in a file share in the Azure portal.

1. From the Azure Portal, search for *storage accounts* in the search bar and click on **Storage Accounts** from the suggestions.

   ![ws name.](media/4s17.png)
   
1. Select the **fslogix{deploymentid}** storage account which was created while creating the NMM account.

   ![ws name.](media/4s18.1.png)
   
1. Select **Fileshare** from the left side menu.

   ![ws name.](media/4s19.1.png)
   
1. Click on the **fsprofilestore** file share.

   ![ws name.](media/4s20.png)
   
1. You will see the user folder created in the file share, click on the folder.

   ![ws name.](media/4s21.png)
   
7. Now you will be able to see the user profiles data stored in the filesharers in a ***.vhd*** format.

   ![ws name.](media/4s22.png)
     
14. Click on the **Next** button present in the bottom-right corner of this lab guide. 
    
