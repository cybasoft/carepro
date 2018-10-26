# Change log

## Version 2.2.0 | 17 Oct 2018

* Added internationalization. User can  select languages defined in the system.
* Added documentation <http://your-domain.com/docs>

## Version 2.1.9 | 8 Oct 2018

* Fresh new look! A cleaner looking theme
* Fixed modals
* Updated WYSIWYG editors
* Fixed minor issues on parent's dashboard
* Improved database queries and performance
* Added debugger for developers
* Added search tool to checked-out children
* Upgraded news module
* Re-designed rooms
* Re-designed child invoice tab
* Added database seeders for children, users and news
* Added news categories

## Version 2.1.8 | Sep 2018

* Added - simple file manager
* Minor bugs and fixes

## Version 2.1.7.4 | Sep 2018

* Added messages module
* Improved mailer performance

## Version 2.1.7.3 | 6 Sep 2018

* Fixed - Missing fields on user update
* Fixed - Missing parent's detaisl in child's page
* Fixed - Error updating food preference
* Added - Ability to delete food intake records
* Added - Parents can update food preferences
* Minor design updates

## Version 2.1.7.2 | 29 Aug 2018

* Fixed - unable to delete user

## Version 2.1.7.1 | 18 Aug 2018

* Fixed - users registration defaults to parent
* Fixed - user form values not persisting on failed validation
* Fixed - registration redirecting to login

## Version 2.1.7 | 17 Aug 2018

* Fixed - translations
* Fixed - 404 errors on  some Linux hosts
* Fixed - migration refresh issue
* Fixed - file module notifications
* Fixed - news modules
* Fixed - issues with installations
* Fixed - unable to update child's information

## Version 2.1.6 | 13 Aug 2018

* Added modals for child's health module
* Added medication administration log
* Added images uploader to attach to medication record for pill identification
* Added ability to write notes in rooms
* Added modal form for health section
* Added ability to delete a photo in full-screen
* Added ability to force running migration in production environment. Just use php index.php migration run force
* Added lockscreen timeout option in settings
* Added child checkin/out option inside a child's record
* Added settings option to control whether a child can be checked in over more than a day
* Tawkto integration for in-app chat
* Added form persistence to allow retaining data in forms when validation fails
* New login/registration design
* Custom background for login in settings
* Fixes to parent's account
* You can now turn on/off paypal or Stripe payment method
* You can add pre-defined invoice terms in settings>billing
* Improved query performance issues
* Updated profile page
* Updated events and calendar pages
* Added a simple file manager to save forms and templates you need to share with staff
* Fresh sidebar navigation icons
* Added notes to rooms
* Fixed migration issues
* Added ability to refresh migrations

## Version 2.1.5

* Updated rooms design
* Updated children page
* Added medication photos for pill identification
* General UI improvements
* Bug fixes and performance improvements

## Version 2.1.4 | 20 July 2018

* Bug fixes

## Version 2.1.3 | 19 July 2018

* Fixed child registration modal
* Fixed auth routes
* Fixed PHP 7.1 & 7.2 compatibility issues

## Version 2.1.2 | 23 June 2018

* Application settings are now loaded from database
* General site settings can be updated by an admin from within the application
* Added billing settings
* Added theme settings to customize colors with custom CSS
* Organized upload folders (see upgrade instructions)
* Added JPG and JPEG extensions for logo and invoice logo
* Renamed children groups to rooms
* Generate children attendance based on a date range
* Attendance reports includes total hours child was checked in for each day
* General interface update
* Fixed issues with manual SQL script
* Fixed required fields issue
* Fixed attendance reporting issue
* Fixed password reset issue
* Fixed alert messages issue

## Version 2.1.1 | 14 June 2018

* Added ability to assign children and staff to rooms
* Checked in children now show a timer
* Staff can only view/edit/update children in their rooms but can checkin/out
* Printable children roster. (Active children, inactive children, daily attendance, all registered children)
* New daily attendance roster
* Added allergy and medication warning icons on children list
* Added an optional 'nickname' field for a child
* Design improvements
* Few bug fixes

Known issues: If you are using PHP v7.2 and encountering count() errors, please downgrade to php v7.1 temporarily while we work on fixing it.

## Version 2.1.0 | 6 June 2018

* Now parents can pay using PayPal!
* Added photo album for each child with a slideshow player
* Added ability to include images/videos in child's daily notes
* Added a tab for listing inactive children
* Added photos for incident reports. Upload photos related to the incident after you record it.
* Added child's attendance pagination
* Printing children list highlights inactive children
* Updated child's registration page
* Updated child's admin page
* now run 'php index.php migration run' to run all latest migration (no need for version unless you wish to rollback)
* Updated lockscreen. Now you will return where you left off before privacy lockscreen.
* Users admin page now shows user photo thumbnail
* Fixed broken photos showing if no image is present.
* Fixed forgotten password blank page
* Fixed issue with updating user information by admin
* Performance improvements and code clean up

## Version 2.0.9 | 17 April 2018

* Integrated Stripe payment gateway. Parents can pay invoices from their account and managers can process credit cards from a child's account. Stripe account required.
* Updated language files
* Updated parent's dashboard
* Removed `config.php` and `database.php` from `/application/config`. These files must be located inside production and development directories in `/application/config/`.
* Minor design changes
* Fixed issue with health tabs not showing in some installations.
* Fixed issue with creating new user.
* General performance improvements.

## Version 2.0.8 | 8 March 2018

* Added religion, ethnicity, birthplace to child's demographics
* Fixed issue with problem list item deletion

## Version 2.0.7 | 19 February 2018

* Fixed – parent’s view- child gender not reflecting gender in database
* Added – Problem list in child’s view tab

## Version 2.0.6 | 8 January 2018

* Invoices can be downloaded as PDF
* You can now email parents their children’s invoices
* Added notifications to parents when any data is added on their child such as invoice, notes, medication, incident reports, food preferences, contacts, providers or authorized pick-up user
* Added notification to admin when a parent registers or new user is registered
* Fixed invoice printing/download
* Fixed compatibility issue with Linux servers
* Minor bug fixes

## Version 2.0.5 | 3 January 2018

* Added parent’s module.

- Parents can now view their own children and allows them to add authorized pickup users.

1. View notes and incident reports.

1. View daycare calendar

1. Update their own profile (address, phone, password)

1. Add medications
1. Add allergies
1. Add food preferences
1. Add emergency contacts
1. Add healthcare providers
1. CANNOT make any deletions
* Completed application translation
* Added email notification for child checkin/out
* Sidebar navigation now showing active page
* Minor fixes of language files
* Minor fixes on email template files
* Fixed – invoice search not returning data* Fixed – sidebar toggle not working
* Completed application translation
* Minor design improvements
 Digital Technologies | https://amdtllc.com | info@amdtllc.com

## Version 2.0.4 | 1 January 2018

* Updated forgot password email template
* Added email settings in config.php
* Fixed - not sending forgot password email
* Fixed - sql file not creating payment_methods table
* Fixed - forgot password page not showing
* Fixed - reset password not showing

## Version 2.0.3 | 21 December, 2017

* Upgrade to use Codeigniter 3.1.6
* Upgraded child module o Updated invoicing o Added healthcare providers tab o Added incident report tab on notes o Added contacts o Updated pickup contacts o Social security number is not national ID# to support other countries
* New login page look
* Configuration settings are now in application/config/config.php. Setting table removed
* Updated authentication module
* Implemented new CI encryption. Please decrypt your data before transferring children database.
* Updated language translation file
* Replaced child emergency tab with contacts
* Switched database engine from MyISAM to InnobDB
* Invoice payments are now entered manually
* Fixed printable children roster
* Fixed calendar
* Updated news module
* Improved database performance
* Removed parents access (temporary). This is being updated and will be available in the next few releases
* Discontinues help module
* Removed landing page
* Discontinued in-app messaging
* Discontinued to-dos
* Removed subscription and membership database  Discontinued saving payment methods on server
* Removed daterangepicker, datepicker, timepicker and color plugins
 Digital Technologies | https://amdtllc.com | info@amdtllc.com
* Removed multitenancy support including company database table.  Discontinued broadcast module

## Version 1.21 | 26 October, 2016

* Updated dashboard landing page
* Fixed invoice not updating status using manual update
* Remove credit card option to save payment methods for a child
* Minor bug fixes

## Version 1.2 | 21 October, 2016

* Fixed child checkout error
* Fixed pickup user information not persisting
* Fixed login issue
* To update from version 1.0, simply copy and replace controller, model and view directories.
* Pay attention if you have made any modifications to any files here as they will be overwritten.

## Version 1.0 | 22 August, 2016

* Initial public release