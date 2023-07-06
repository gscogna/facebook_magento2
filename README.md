facebook_magento2
The official plugin is deprecated. the developers have decided to switch to new plugin. The new plugin is https://github.com/magento/meta-for-magento2 "declared" compatible with older versions of magento and php. I managed to make it compatible with older versions.
this module work with "facebook/php-business-sdk": "^15.0.0" dont forget to update.
https://github.com/facebook/facebook-php-business-sdk/tree/main


Create Folder Meta

Save the zip file and put it in app/code/Meta

php bin/magento setup:upgrade

php bin/magento setup:di:compile

php bin/magento setup:static-content:deploy -f

php bin/magento indexer:reindex

php bin/magento cache:clean

php bin/magento cache:flush
