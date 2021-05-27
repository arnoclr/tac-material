# Tarteaucitron Material Theme

New snackbar design (only bottom) :
![Cookie Banner](https://i.imgur.com/FCkOW5A.png)

Services dialog also comes with refreshed UI :
![Services Dialog](https://i.imgur.com/6jnxIDZ.png)

HTML code :

```html
<head>
    ...
    <link rel="stylesheet" href=".../tarteaucitron.min.css">
</head>

<body>
    ...
    <script src="https://cdn.jsdelivr.net/gh/AmauriC/tarteaucitron.js@1.8.4/tarteaucitron.min.js"></script>
    <script>
        tarteaucitron.init({
            "privacyUrl": "", /* Privacy policy url */

            "hashtag": "#tarteaucitron", /* Open the panel with this hashtag */
            "cookieName": "tarteaucitron", /* Cookie name */

            "orientation": "bottom", /* Banner position (top - bottom - middle - popup) */

            "groupServices": true, /* Group services by category */

            "showAlertSmall": false, /* Show the small banner on bottom right */
            "cookieslist": false, /* Show the cookie list */
            
            "showIcon": false, /* Show cookie icon to manage cookies */
            // "iconSrc": "", /* Optionnal: URL or base64 encoded image */
            "iconPosition": "BottomRight", /* Position of the icon between BottomRight, BottomLeft, TopRight and TopLeft */

            "adblocker": false, /* Show a Warning if an adblocker is detected */

            "DenyAllCta" : true, /* Show the deny all button */
            "AcceptAllCta" : true, /* Show the accept all button when highPrivacy on */
            "highPrivacy": true, /* HIGHLY RECOMMANDED Disable auto consent */

            "handleBrowserDNTRequest": false, /* If Do Not Track == 1, disallow all */

            "removeCredit": false, /* Remove credit link */
            "moreInfoLink": true, /* Show more info link */
            "useExternalCss": true, /* If false, the tarteaucitron.css file will be loaded */

            //"cookieDomain": ".my-multisite-domaine.fr", /* Shared cookie for subdomain website */

            "readmoreLink": "", /* Change the default readmore link pointing to tarteaucitron.io */
            
            "mandatory": true /* Show a message about mandatory cookies */
        });
    </script>
</body>
```

You can customize colors (the blue accent color) with css variables. 

```css
:root {
    --snackbar-link-color: #669df6;
    --snackbar-primary-color: #1a73e8;
    --snackbar-border-radius: 4px;
}
```