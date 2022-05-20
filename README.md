# SEO Magento 2 Category Image Alt Tag
Set Custom Category Image Alt to catalog category images for SEO purpose.
<br/>
By default Magento 2 has only these category attributes under Search Engine Optimization.

![search_engine_optimization](https://user-images.githubusercontent.com/14094984/66201033-ecb12b80-e6d4-11e9-9c22-2921a28a2643.png)

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

4. Go to Admin > Catalog > Categories >  Select any category which you like to specify a category image alt text.

![category_image_alt](https://user-images.githubusercontent.com/14094984/66200814-6e548980-e6d4-11e9-96ba-cc739da6634c.png)

<br/>

## Example

![sample_earl](https://user-images.githubusercontent.com/14094984/66201312-a27c7a00-e6d5-11e9-9163-cc582b67d5ff.png)

<br/>

## Requirements
Magento 2.4.x Community

<br/>

## Changelog
### [Version 2.0.0] (2019-10-4)

### [Version 2.0.1] - (2022-20-5)
#### Improved
- Refactored the custom module for Magento 2.4.x