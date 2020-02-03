## Edit your site information

Change the name of your collection
1.  Click on **Settings**
2. Click on **Collection**
3. Change the name of your collection
4. **Save**

![](https://github.com/huridocs/uwazi/blob/802decbd51a1b8726ee61801cd5d224e336b525d/Collection%20Name%20Screenshot.png)

## Make your collection private

If you are handling sensitive information or you just want your collection to be accessible only via login, you can configure Uwazi to do so. 

1. Click on **Settings**
2. Click on **Collection**
3. Click the checkbox to make the instance private

![](https://github.com/huridocs/uwazi/blob/quincywiele-patch-2/Private%20Instance.png)

# Landing page
The landing page is the first thing users will see when visiting your Uwazi instance. By default, your landing page is the Library, without any filter applied and a list with all documents and entities.

However you can use any page from your Uwazi instance as a landing page, just copying and pasting the URL on the text box below custom page.

These are some examples:

- A [static page](https://github.com/huridocs/uwazi/wiki/Create-pages): `/page/dicxg0oagy3xgr7ixef80k9`
- A [library query](https://github.com/huridocs/uwazi/wiki/Filter): `/library/?searchTerm=test`
- A document or entity: `/document/4y9i99fadjp833di` `/entity/9htbkgpkyy7j5rk9`

Always use URLs relative to your site, starting with / and skipping the `https://yoursite.com`.

# Advanced settings

## Mailer configuration

This is a JSON configuration object that should match the options values required by Nodemailer, as explained [here](http://nodemailer.com/smtp/).

This setting takes precedence over all other mailer configuration. If left blank, then the configuration file in `/api/config/mailer.js` will be used.

## Google Analytics

You can use Google Analytics to track website visits by adding your [Google Analytics ID](https://support.google.com/analytics/answer/3123666?hl=en) to Uwazi under Settings > Collection. 

![Google Analytics field](https://raw.githubusercontent.com/huridocs/uwazi-assets/master/wiki/screenshots/analytics.jpg) 

## Custom header

Sadly is not possible to edit your header from Settings right now, but we will work to make it available soon. Meanwhile, you can create an [issue](https://github.com/huridocs/uwazi/issue/) and we will customise the header background image for you.

Requirements:

- Your logotype in PNG format (transparent background) and 72px height. Width is not fixed, but limited to 288px, so you can play until that size.
- Your brand colour to change the header background.

We will upload all the changes it for you once you have the final design.

![CEJIL](http://huridocs.github.io/uwazi-assets/wiki/screenshots/site-cejil.png)

Our partner [CEJIL](https://cejil.uwazi.io) is a great example of landing page and header customization.