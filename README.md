# extensions-hmvc

## Modular Extensions installation
Start with a clean CI install
Set $config[‘base_url’] correctly for your installation
Access the URL /index.php/welcome => shows Welcome to CodeIgniter
Drop Modular Extensions third_party files into the CI 2.0 application/third_party directory
Drop Modular Extensions core files into application/core, the MY_Controller.php file is not required unless you wish to create your own controller extension
Access the URL /index.php/welcome => shows Welcome to CodeIgniter
Create module directory structure application/modules/welcome/controllers
Move controller application/controllers/welcome.php to application/modules/welcome/controllers/welcome.php
Access the URL /index.php/welcome => shows Welcome to CodeIgniter
Create directory application/modules/welcome/views
Move view application/views/welcome_message.php to application/modules/welcome/views/welcome_message.php
Access the URL /index.php/welcome => shows Welcome to CodeIgniter
You should now have a running Modular Extensions installation.
## Installation Guide Hints:
-Steps 1-3 tell you how to get a standard CI install working - if you have a clean/tested CI install, skip to step 4.
-Steps 4-5 show that normal CI still works after installing MX - it shouldn’t interfere with the normal CI setup.
-Steps 6-8 show MX working alongside CI - controller moved to the “welcome” module, the view file remains in the CI application/views directory - MX can find module resources in several places, including the application directory.
-Steps 9-11 show MX working with both controller and view in the “welcome” module - there should be no files in the application/controllers or application/views directories.
