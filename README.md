#LATCH INSTALLATION GUIDE FOR DRUPAL 8


##PREREQUISITES 
 * Drupal version 8.0.0 or later (Tested up to 8.2.3).

 * Curl extensions active in PHP (uncomment **"extension=php_curl.dll"** or **"extension=curl.so"** in Windows or Linux php.ini respectively. 

 * To get the **"Application ID"** and **"Secret"**, (fundamental values for integrating Latch in any application), it’s necessary to register a developer account in [Latch's website](https://latch.elevenpaths.com"https://latch.elevenpaths.com"). On the upper right side, click on **"Developer area"**.

 
##DOWNLOADING THE DRUPAL 8 PLUGIN
 * When the account is activated, the user will be able to create applications with Latch and access to developer documentation, including existing SDKs and plugins. The user has to access again to [Developer area](https://latch.elevenpaths.com/www/developerArea"https://latch.elevenpaths.com/www/developerArea"), and browse his applications from **"My applications"** section in the side menu.

* When creating an application, two fundamental fields are shown: **"Application ID"** and **"Secret"**, keep these for later use. There are some additional parameters to be chosen, as the application icon (that will be shown in Latch) and whether the application will support OTP  (One Time Password) or not.

* From the side menu in developers area, the user can access the **"Documentation & SDKs"** section. Inside it, there is a **"SDKs and Plugins"** menu. Links to different SDKs in different programming languages and plugins developed so far, are shown.


##INSTALLING THE MODULE IN DRUPAL 8
* Add the module in the administration panel in Drupal 8. Unzip the downloaded plugin and place the whole content inside **"modules"**.

* Go to **"Extend"** in the up side menu. Search for Latch module and enable it.

* Insert **"Application ID"** and **"Secret"** data, generated before in the **"Latch settings"** options that will be shown in the **"Configuration"** tab in the up side menu.

* Once the module is installed, a new **"Latch account"** button will be shown under **"My account"**. The token generated by the Latch app will be added there.

* Go to **"Permissions"** from **"People"** menu, and access Latch permissions, are all under **"Latch"**. At least **"pairing the account with Latch"** option should be enabled corresponding to **"authenticated user"** permissions.


##UNINSTALLING THE MODULE IN DRUPAL 8
* From **"Extend"** go to **"Uninstall"** tab, and select Latch. Press **"Uninstall"** and press again on **"Uninstall"** to confirm.

* Latch is still in the module list, but **"Application ID"** and **"Secret"** have been removed, so if activating it again they will have to be introduced again.


##USE OF LATCH MODULE FOR THE USERS
**Latch does not affect in any case or in any way the usual operations with an account. It just allows or denies actions over it, acting as an independent extra layer of security that, once removed or without effect, will have no effect over the accounts, that will remain with its original state.**

###Pairing a user in Drupal 8
The user needs the Latch application installed on the phone, and follow these steps:

* **Step 1:** Logged in your own account, go to **"My account"**, and click on the new button **"Latch account"**.

* **Step 2:** From the Latch app on the phone, the user has to generate the token, pressing on **“Add a new service"** at the bottom of the application, and pressing **"Generate new code"** will take the user to a new screen where the pairing code will be displayed.

* **Step 3:** The user has to type the characters generated on the phone into the text box displayed on the web page. Click on **"Pair Account"** button.

* **Step 4:** Now the user may lock and unlock the account, preventing any unauthorized access.


###Unpairing a user in Drupal 8
* From your Drupal 8 account go to the link **“My account”**, tap the **“Latch account"** button, followed by **“Unpair Account”**. Finally, an alert indicating that the service has been unpaired will be displayed.


##RESOURCES
- You can access Latch´s use and installation manuals, together with a list of all available plugins here: [https://latch.elevenpaths.com/www/developers/resources](https://latch.elevenpaths.com/www/developers/resources)

- Further information on de Latch´s API can be found here: [https://latch.elevenpaths.com/www/developers/doc_api](https://latch.elevenpaths.com/www/developers/doc_api)

- For more information about how to use Latch and testing more free features, please refer to the user guide in Spanish and English:
	1. [English version](https://latch.elevenpaths.com/www/public/documents/howToUseLatchNevele_EN.pdf)
	1. [Spanish version](https://latch.elevenpaths.com/www/public/documents/howToUseLatchNevele_ES.pdf)