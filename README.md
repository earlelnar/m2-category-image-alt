# Magento 2 Category Image Alt Tag
Set Custom Category Image Alt to catalog category images. 
</br>

## Installation
1. Download the extension .zip file and extract the files.
2. Copy the extension files folder to the {magento2-root-dir}/app/code
3. Run the following series of command from SSH console of your server:
```
 php bin/magento maintenance:enable
 rm -rf var/cache/;  rm -rf var/di/;  rm -rf generated/;  rm -rf var/view_preprocessed/;  rm -rf pub/static/*;
 php bin/magento setup:upgrade
 php bin/magento setup:static-content:deploy -f
 php bin/magento cache:flush
 php bin/magento setup:clean
 php bin/magento maintenance:disable
```