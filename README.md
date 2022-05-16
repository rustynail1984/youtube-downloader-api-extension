## RajWebConsulting

### YouTube to MP3 Converter and MP4 Downloader API extension.

##### This script is an extension for MP3 Converter Pro v3 from [RajWebConsulting](https://shop.rajwebconsulting.com/store/converter-scripts) and enables you to install Single/Multi Button and Widget APIs on multiple Domains and consuming the JSON API of the Main MP3 Converter Pro v3 installation, to have a SOLID infrastructure (Using File Caching and saving CPU ressources).

- Main Version requires a MP3 Converter Pro v3 License from [RajWebConsulting](https://shop.rajwebconsulting.com/store/converter-scripts)

```diff
> If you don't want to buy a MP3 Converter Pro License and use your own Server resources,
> then please consider using the ready to use Button and Widget APIs (Contains Ads) from my Main Sponsor.

@@ (You don't need to download this Script, if using his APIs.) @@
```

> #### Main Sponsor
> https://ytconvert.me


#### Donations

- Each Donation is helpful. Thank you so much for supporting me.

<a href="https://www.buymeacoffee.com/andre.h1984" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-yellow.png" alt="Buy Me A Coffee" height="41" width="174"></a>

#### Demo
- Please see a running DEMO on the domain of my Main Sponsor.


#### Installation
This package requires Nodejs version 16.15.0 or later to build the app.

1. Download the zip file from Github.

2. install dependencies via yarn.

```bash
yarn install
```

4. rename the .env.example file to .env and edit the example variables
```env
APP_NAME="YouTube to MP3 APIs"
APP_DOMAIN="https://example.com" # Domain where you wantr to install this app
APP_API_URL="https://example.com" # Domain of the ajax.php. usually should be the same as the APP_DOMAIN
``` 

5. Build for production
```bash
yarn build
yarn generate
```

6. Copy `.htaccess` and `ajax.php` files from `server` folder to `dist` folder
 and Add your MP3 Converter Pro v3 domain in the `ajax.php`

```php
// Your MP3 Converter Pro v3 URL here
$baseUrl = 'https://example.com';
```

7. Set your Domain Working directory to `/dist` folder
