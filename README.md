# Auto-IISFtp

Hi All,

One day I have been asked to setup a FTP site on IIS7 and configure user isolation on it.
If you have ever gone through the above requirement, then you might felt pain setting these up.
If not, then please do check below articles from Microsoft which teaches how to address these requirements.


Microsoft Articles:

FTP setup on IIS: https://docs.microsoft.com/en-us/iis/publish/using-the-ftp-service/creating-a-new-ftp-site-in-iis-7
User Isolation in FTP IIS: https://docs.microsoft.com/en-us/iis/publish/using-the-ftp-service/configuring-ftp-user-isolation-in-iis-7

There are lots of settings and steps involved in this process, as this was our regular task which arises with every new server we setup and this time it was me who must do it and it was painful for me, therefor to avoid such pain in future I have created a PowerShell script which will do the same things automatically in background which are mentioned in Microsoft article/required to setup FTP site on IIS with user isolation. You just need to answer the CMD prompts.

Requirement: Setup FTP site on IIS 7 and above
Regular Solution: Perform the steps mentioned in the given Microsoft article
Problem with the regular solution: takes much time and efforts, lengthy process, confusing steps
My Solution: PowerShell script to perform all the steps in few clicks in no time.

What this script will Do?
1.       Script will set up FTP site on IIS
2.       Script will handle the necessary folder security permissions
3.       Script will configure FTP site logging with all w3c fields
4.       Script will create the FTP IIS manager users with appropriate permissions
5.       Script will handle all the authorization rules
6.       Script will take care of authentication method
7.       Script will take care of user isolation
8.       Script can be used to add more users to existing FTP sites
9.       Script can be used to create FTP site with default values (FTP site name, folder, user credential all will be default which are given with this article)
10.   Script can be used to create FTP site with all custom data. (You will need to provide all details like user credential, name for site, folder path etc. by answering simple CMD Prompts)
