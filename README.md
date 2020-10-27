List Azure subscription's administrators
========================================

            
What is proposed

You'll find in this function an easy way to extract the list of administrators level accounts assigned on your Azure subscriptions within an authenticated PowerShell Azure session. It will look for Owner and everything with Administrator in the role names.


 

Overview

 

   You will end up with an output in the like of:

 



PowerShell
Edit|Remove
powershell
Fetching administrators for subscription: sub1
Fetching administrators for subscription: sub2

Name                           Value
----                           -----
subscription                   sub1
admins                         {@{ObjectId=17b7df4e-bf37-469b-8708-7d2386efd850; SignInName=; DisplayName=MS-PIM; Sc...
subscription                   sub2
admins                         {@{ObjectId=17b7df4e-bf37-469b-8708-7d2386efd850; SignInName=; DisplayName=MS-PIM; Sc...

Fetching administrators for subscription: sub1 
Fetching administrators for subscription: sub2 
 
Name                           Value 
----                           ----- 
subscription                   sub1 
admins                         {@{ObjectId=17b7df4e-bf37-469b-8708-7d2386efd850; SignInName=; DisplayName=MS-PIM; Sc... 
subscription                   sub2 
admins                         {@{ObjectId=17b7df4e-bf37-469b-8708-7d2386efd850; SignInName=; DisplayName=MS-PIM; Sc...




 

Requirements

Tested with Az.Accounts Version 1.x


        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
