# How-to-install-Gline-Jar-modules
User manual to install and activate Gline Jar module

Step 1: install the gline.pem into workbench
Click Tools and select Certificate Management. Click the User Trust Store and import the gline certificate file.
<img width="2687" height="613" alt="image" src="https://github.com/user-attachments/assets/a7e22843-cc3b-4b93-8f41-d96aefe4503c" />

Step 2: install gline.pem into station platform
Even in the same PC where has installed gline.pem in workbench, this step is still mandatory.
Go to Platform and click the Certificate Management. Then click the User Trust Store. Import the gline certificate file again. 
<img width="1899" height="413" alt="image" src="https://github.com/user-attachments/assets/b9ca0742-f7ac-4cb1-aba5-7d5638f5e2fc" />

Step 3: close the workbench and add the gline modules into the workbench module folder. 

Step 4: install the platform daemon. This will adopt the new certificate to the workbench. 

Step 5: install the gline module into the Niagara station module. This is similar to other 3rd jar module import porcess. Go the platform and software manager and import the module file. Then reboot the station. 
If the station is running as supervisor at the same workbench, this step is not necessary. 

With above steps, you could then enjoy our modules. 

If you have any issue, feel free to contact with me jason.zhang@gline-net.com


