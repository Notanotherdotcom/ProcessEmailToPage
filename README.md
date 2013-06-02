# ProcessWire2.3+ ProcessEmailToImage

This module allows you to email text and images (as attachments) to multiple sections of your site.

To use it, extract the attached zip file into your /site/modules/ directory and check for new modules in the ProcessWire Admin area, then install the module.

Once installed, go to configure the module.

You will need to set up an email account for each "category" (page parent) you want to have emails processed to. These must all be on the same server - either local or remote is fine. Once these are set up, enter your email password (same for each account) as well as type (POP3/IMAP) host and port information, then tick the box if you want new pages to be automatically published (default is unpublished).

For each category, you can now enter an email address, category (page parent) and even template for the page (the system will rely on you specifying a page parent that allows new children using the template you have selected, so take care!). To add more email address/category combinations click on the "Add another category" button to add more.

Next, you can optionally set up delimiters to split the email's content into different text fields - useful if you want part of your email to be in the body area and some in the sidebar for example. This part is fairly self-explanatory in the config screen.

Final note - the module will attempt to add attachments to an images field, so make sure you still have that default field!

There are more things that need to be added - more checks for attachment types and a whitelist - but for now it should be functional and fun to use!

*Full details of this module are available here: http://modules.processwire.com/modules/process-email-to-page/*

__Notes:__

* This module contains a third-party library - Flourishlib - which is subject to its own license: http://flourishlib.com/docs/LicenseAgreement

__Updates:__

* v1.0.0 - first release.