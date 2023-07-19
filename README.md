# Tiny theme - Add Tinylytics

**NOTE:** This plugin is for Tinylytics users. It is designed to work out-of-the-box with the [Tiny Theme for Micro.blog](https://tinyformicro.blog), but other Micro.blog theme developers can add compatibility to their theme as well.

![Tiny Theme Head Graphic](https://github.com/MattSLangford/Tiny-theme-Tinylytics/blob/main/screenshot.jpg?raw=true)

### What it does
Adds all Tinylytics features to your site:

- Analytics
- Hit Counter
- Kudos Button

### Installation and Setup

#### To Start Tracking Traffic & Enable Kudos
1. Install from the Micro.blog plugins page
2. Click Settings next to the newly installed plugin
3. Add your Tinlytics ID and Emoji


#### Shortcodes for Hits and Uptime
You can optionally show a hit counter (free and paid Tinylytics accounts) or uptime viewer (paid Tinylytics accounts only) for your overall site by using the following shortcodes in any post or page. You can also show hits for a specific post/page by using the `hitsx` shortcode.

`{{< hits >}}`
`{{< hitsx >}}`
`{{< uptime >}}`


### For Theme Developers

You can support this plugin directly within your theme by adding the following snippet in your theme files:

```
{{ if templates.Exists "partials/plugin_tinylytics.html" }}
	  <button class="tinylytics_kudos">Kudos</button>
{{ end }}
```

This checks to see if the plugin is installed. If it is, it adds a Kudos button. In this example, "Kudos" is simply fallback text until the Tinylytics script loads.
