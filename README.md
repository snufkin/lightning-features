lightning-features
==================
[![Build Status](https://travis-ci.org/acquia/lightning-features.svg?branch=7.x-1.x)](https://travis-ci.org/acquia/lightning-features)

Decoupled components used by the Lightning distribution for Drupal.

Using the lightning_features module in your own install profile's is recommended.

FAQ

- If you are not using a module and no lightning_features modules inuse require it as a dependency, it could be deleted from your project with a patch for lightning_features.make
- You will not see any performance decrease on your delivery if you leave uninstalled modules in your profiles directory.
- We recommend evaluating each lightning_* module for your own usage and only using the things you deem necessary.

See lightning_features.make for a detailed list of dependent modules and libraries.

### Updating
If you downloaded the Lightning Demo from http://drupal.org/project/lightning

`cd profiles/lightning/modules/contrib/lightning_features`

`sh update.sh`

If you built your own profile using Lightning Features: you must keep lightning_features and the contrib it provides in profiles/[my-profile]/modules/contrib otherwise the update.sh script will not run correctly.

`cd profiles/[my-profile]/modules/contrib/lightning_features`

`sh update.sh`

### Behat Tests

Run tests from the command line:

`sh run-tests.sh http://lightning.local`

Replace [http://lightning.local] with the site environment url to test against.

#### lightning_article

* Article content type exists
* Creating an article as admin
* Article content type has fields provided by feature

#### lightning_breakpoints

* Checks to ensure breakpoints were created

#### lightning_cache

* Checks to ensure Views Content Cache is enabled

#### lightning_filter

* Text formats exist
* Text formats have appropriate feature-defined filters

#### lightning_forms

* Webform type present
* Can create Webform
* Check basic Webform fields

#### lightning_fpp

* Checks for FPP types
* Checks for fields on FPP types

#### lightning_identifiers

* Checks to ensure taxonomy exists

#### lightning_landing

* Ensure landing page content type exists
* Create landing page content
* Landing Page fields

#### lightning_letterbox

* Checks for letterbox breakpoints

#### lightning_moderation

* Ensure moderation steps are created

#### lightning_page

* Ensure page content type exists
* Create page content
* Page fields

#### lightning_roles

* Role exists: curator
* Role exists: reviewer
* Role exists: marketer

#### lightning_sps

* Checks for Article field collection

#### lightning_tags
* Tags taxonomy vocabulary exists

#### lightning_wysiwyg

* Check Linkit exists
* Linkit sanity check
