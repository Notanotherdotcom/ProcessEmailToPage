# ProcessWire2.3+ ProcessEmailToImage

This module allows you to email text and images (as attachments) to multiple sections of your site.

To use it, extract the attached zip file into your /site/modules/ directory and check for new modules in the ProcessWire Admin area, then install the module.

Once installed, go to configure the module.

You will need to set up an email account for each "category" (page parent) you want to have emails processed to. These must all be on the same server - either local or remote is fine. Once these are set up, enter your email password (same for each account) as well as type (POP3/IMAP) host and port information, then tick the box if you want new pages to be automatically published (default is unpublished).

For each category, you can now enter an email address, category (page parent) and even template for the page (the system will rely on you specifying a page parent that allows new children using the template you have selected, so take care!). To add more email address/category combinations click on the "Add another category" button to add more.

Next, you can optionally set up delimiters to split the email's content into different text fields - useful if you want part of your email to be in the body area and some in the sidebar for example. This part is fairly self-explanatory in the config screen.

The module will add attachments to an images field, and optionally embed images into the text body to match the email layout. Attachments will be separated into image and non-image types.

PW users can be identified by the email address and the created/modified values set to the user. Creation of new pages can be limited to only matched users.

Creation of a new page can trigger a notification email to chosen PW users.

You can optionally set up a host whitelist - this is the actual smtp host that the email comes from - it is not extracted from the email address.


*Full details of this module are available here: http://modules.processwire.com/modules/process-email-to-page/*

__Notes:__

* This module contains a third-party library - Flourishlib - which is subject to its own license: http://flourishlib.com/docs/LicenseAgreement

__Updates:__

* v1.0.0 - first release.
* v1.0.1 - various bug fixes including php notices
* v1.0.2 - force secure option and fix for plain text vs html emails
* v1.0.9 - Improved image handling - inline, related, embedded. Can also optionally embed images in the body field. Also, image and body fields are now configurable.
* v1.1.0 - Added support from date received and from details
* v1.1.1 - Separate "From" into name, email, and user matching
* v1.1.2 - Set created and modified user ids for the new page based on a match to a PW user.
* v1.1.5 -  Added a LOT of new config options and support for mail notification of newly added pages.