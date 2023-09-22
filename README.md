# Tiny theme - Add Tinylytics

**NOTE:** This plugin is for Tinylytics users. It is designed to work out-of-the-box with the [Tiny Theme for Micro.blog](https://tinyformicro.blog), but other Micro.blog theme developers can add compatibility to their theme as well.

![Tiny Theme Head Graphic](https://github.com/MattSLangford/Tiny-theme-Tinylytics/blob/main/screenshot.jpg?raw=true)

### What it does
Adds all Tinylytics features to your site:

- Analytics
- Hit Counter
- Kudos Button
- Webring

### Installation and Setup

#### To Start Tracking Traffic & Enable Kudos
1. Install from the Micro.blog plugins page
2. Click Settings next to the newly installed plugin
3. Add your Tinlytics ID and Emoji


#### Shortcodes for Hits and Uptime
You can use shortcodes in your Micro.blog posts and pages to display styled statistics. There are 4 shortcodes available:

1. `{{< hits >}}` - Shows total hits for all pages on your site.
2. `{{< hitsx >}}` - Shows hits only for the current page.
3. `{{< uptime >}}` - Shows your site's uptime %. Requires a Tinyltyics **paid** account and additional setup in Tinylytics.
4. `{{< countries >}}'` - Shows a list of countries that have visited your site in emoji form
5. `{{< webring >}}` - Shows a link to the Tinylytics webring*

*This also enables the ability to include custom webring links. For example you can add `<a href="#" target="_blank" class="tinylytics_webring">Tinylytics Webring 🕸️💍</a>` to your site in any location, customizing the **displayed text** at will.

### For Theme Developers

You can support this plugin directly within your theme by adding the following snippet in your theme files:

```
{{ if templates.Exists "partials/plugin_tinylytics.html" }}
	  <button class="tinylytics_kudos">Kudos</button>
{{ end }}
```

This checks to see if the plugin is installed. If it is, it adds a Kudos button. In this example, "Kudos" is simply fallback text until the Tinylytics script loads.

## Do you value this theme and plugins?

Tiny Theme and its plugins are provided free of charge to Micro.blog users. I do not receive payment from Micro.blog in any way. If you'd like to help offset expenses and ensure the future of Tiny Theme and its plugins, please consider supporting its development.

[Make a one-time Donation](https://donate.stripe.com/5kAeV7gWk9fk7aE7ss) in any amount or [setup a $5 monthly donation](https://buy.stripe.com/28odR3eOc2QWeD6cMN). Thank you!


