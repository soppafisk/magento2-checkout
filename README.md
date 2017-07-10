Svea checkout for Magento2

* Requirements (inherited from dependencies)*
* Magento 2.1.4 or above
* PHP 5.6 >=
* php-soap
* php-curl

*Installation:*

run `composer require sveaekonomi/magento2-checkout && composer install` to install files.
Then run `bin/magento setup:db:upgrade && bin/magento setup:ci:compile && bin/magento cache:flush` from your base folder 
to install database scripts and recompile the dependency injections and clear cache.

Head to _administration -> Stores -> Configuration -> Payment methods -> Svea Ekonomi Checkout_


and enable it, provide your integration authentication details and choose order-statuses to be used 
before as well as after order acknowledgement. Save and clear cache.

