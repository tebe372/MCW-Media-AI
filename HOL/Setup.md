
# Media AI setup

## Requirements

-   Microsoft Azure subscription

-   Local machine or Azure virtual machine configured with:

-   Visual Studio 2017 Community Edition or later


## Before the hands-on lab

Duration: 30 minutes

In this lab, you will create a developer environment and download the required files for this course if you do not already have one that meets the requirements.

### Prerequisites

1.  Microsoft Azure subscription <http://azure.microsoft.com/en-us/pricing/free-trial/>

2.  Client computer with Windows 7 or later with Visual Studio 2017

### Task 1: Configure a development environment

If you do not have a machine setup with Visual Studio 2017 Community complete this task.

1.  Create a virtual machine in Azure using the **Visual Studio Community 2017 (latest release) on Windows Server 2016 (x64)** image. This is important as you need to have Visual Studio 2017 version 15.4 or later to complete this lab.

    ![In this screenshot, visual studio community 2017 is entered in a search box, and the Visual Studio Community 2017 (latest release) on Windows Server 2016 (x64) row is selected and highlighted in the search results.](images/Setup/image3.png "Use the image above to create a virtual machine in Azure")

It is **highly** recommended to use a DS2 or D2 instance size for this VM.

### Task 2: Disable IE enhanced security

Note: Sometimes this image has IE ESC disabled, and sometimes it does not.

1.  On the new VM, you just created click the Server Manager icon

    ![Server Manager is highlighted on the taskbar.](images/Setup/image4.png "Select Server Manager")

2.  Click Local Server

    ![In Server Manager, Local Server is selected and highlighted in the navigation pane.](images/Setup/image5.png "Select Local Server")

3.  On the right side of the pane, click **On** by IE Enhanced Security Configuration

    ![On is highlighted next to IE Enhanced Security Configuration.](images/Setup/image6.png "Turn IE Enhanced Security Configuration on")

4.  Change to **Off** for Administrators and click **OK**

    ![Off is selected and highlighted under Administrators in the IE Enhanced Security Configuration dialog box, and OK is highlighted at the bottom.](images/Setup/image7.png "Turn Administrators off")

### Task 3: Update Visual Studio Tools for Azure Functions

1.  Open Visual Studio 2017, then click on the **Tools** menu, then click on **Extensions and Updates...**

    ![In Visual Studio 2017, the Tools menu is highlighted and labeled 1, and Extensions and Updates is selected, highlighted, and labeled 2 in the submenu.](images/Setup/image8.png "Select Extensions and Updates")

1.  On the Extensions and Updates dialog, click on **Updates**, then **Visual Studio Marketplace** on the left side of the dialog, then click on **Update** for the **Azure Functions and Web Jobs Tools** extension to update to the latest version

    ![Updates (labeled 1) and Visual Studio Marketplace (labeled 2) are highlighted on the left side of the Extensions and Updates dialog box, and the Update button and the Azure Functions and Web Jobs Tools extension (labeled 3) are selected and highlighted on the right.](images/Setup/image9.png "Update Azure Functions and Web Jobs Tools")

### Task 4: Install Visual Studio Tools for Logic Apps

1.  Within the **Extensions and Updates** dialog within Visual Studio 2017 sill open from the previous task, click on the **Online** category on the left side of the dialog.\
    ![Online is highlighted on the left side of the Extensions and Updates dialog box.](images/Setup/image10.png "Select the Online category")

2.  In the **Search** box in the upper right of the dialog, type in **Azure Logic Apps** to search for the **Azure Logic Apps Tools for Visual Studio** extension. Then click **Download** on the Extension to install it.\
    ![Search Results is highlighted on the left side of the Extensions and Updates dialog box, Azure Logic Apps is highlighted on the top right (labeled 1), and the Download button and the Azure Logic Apps Tools for Visual Studio extension (labeled 2) are selected and highlighted in the middle.](images/Setup/image11.png "Download Azure Logic Apps Tools for Visual Studio")
    

3.  Click **Close** on the **Extensions and Updated** dialog![Search Results is highlighted on the left side of the Extensions and Updates dialog box, Azure Logic Apps Tools for Visual Studio is selected in the middle, and Close is highlighted on the bottom right.](images/Setup/image12.png "Close the Extensions and Updated dialog box")

4.  Close Visual Studio, the pending installation of the Azure Logic Apps Tools for Visual Studio will automatically launch

5.  On the **VSIX Installer** dialog, click on **Modify**\
    ![Modify is highlighted at the bottom of the VSIX Installer dialog box.](images/Setup/image13.png "Select Modify")

6.  Wait for the extension to be installed, this should only take about 1 minute\
    ![A progress bar is displayed in the VSIX Installer dialog box.](images/Setup/image14.png "Wait for the extension to install")

7.  Once installation is complete, click **Close**\
    ![A Modifications Complete message is displayed in the VSIX Installer dialog box.](images/Setup/image15.png "Close the installer")

8.  Restart Visual Studio now that the extension has been installed

### Task 5: Validate connectivity to Azure

1.  From within the virtual machine, Launch Visual Studio 2017 and validate that you can login with your Microsoft Account when prompted

2.  Validate connectivity to your Azure subscription. Launch Visual Studio, open Server Explorer from the View menu, and ensure that you can connect to your Azure subscription

    ![An Azure subscription is highlighted in Server Explorer, and the submenu is displayed with an option to connect to your Azure subscription.](images/Setup/image16.png "Validate connectivity")

### Task 6: Download the exercise files 

1.  Download the exercise files for the training (from within the virtual machine)

    a.  Create a new folder on your computer named **C:\\Hackathon**

    b.  Download the support files (.zip format), <https://cloudworkshop.blob.core.windows.net/media-services-and-cdn/Media-Services-Student-Files.zip> to the new folder.

    c.  Extract the contents to the same folder
