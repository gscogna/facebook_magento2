facebook_magento2
The official plugin is deprecated. the developers have decided to switch to new plugin. The new plugin is https://github.com/magento/meta-for-magento2 "declared" compatible with older versions of magento and php. I managed to make it compatible with older versions. If you want to offer me a coffee at paypal link https://www.paypal.com/donate/?hosted_button_id=GGH3W7A9U8GAG, thanks.

Create Folder Meta

Save the zip file and put it in app/code/Meta

php bin/magento setup:upgrade

php bin/magento setup:di:compile

php bin/magento setup:static-content:deploy -f

php bin/magento indexer:reindex

php bin/magento cache:clean

php bin/magento cache:flush
