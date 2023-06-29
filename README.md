# Tiny theme - Add Tinylytics

**NOTE:** This plugin is for PAID [TINYLYTICS](https://tinylytics.app) USERS ONLY. It is designed to work out-of-the-box with the [Tiny Theme for Micro.blog](https://tinyformicro.blog), but theme developers can add compatibility to their theme as well.

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
3. Add your Tinlytics ID and Emoji (for kudos*)

*Kudos is a paid Tinylytics feature. If you are not a paid user, do not use this plugin.

#### To Add a Publicly Visible Hit Counter
You can optionally show a hit counter for your overall site by using the following shortcode in any post or page.

`{{< hits >}}`

### For Theme Developers

You can support this plugin directly within your theme by adding the following snippet in your theme files:

```
{{ if templates.Exists "partials/plugin_tinylytics.html" }}
	  <button class="tinylytics_kudos">Kudos</button>
{{ end }}
```

This checks to see if the plugin is installed. If it is, it adds a Kudos button. In this example, "Kudos" is simply fallback text until the tinylytics script loads.
