---
title: Themes
id: themes
layout: manual
description:  In addition to the built-in themes, custom themes can be defined to enable complete control over the look and style of the terminal window.
---
Tilix supports themes for configuring the color scheme of the terminal, each theme is stored in a file. A theme file is a simple json file that specifies the color for each element as well as identifying whether certain colors should be used or defaulted. Here is an example of a theme file:

{% highlight json %}
{
    "name": "Orchis",
    "comment": "Tango but using Orchis foreground/background colors",
    "foreground-color": "#EFEFEF",
    "background-color": "#303030",
    "use-theme-colors": false,
    "use-highlight-color": false,
    "highlight-foreground-color": "#ffffff",
    "highlight-background-color": "#a348b1",
    "use-cursor-color": false,
    "cursor-foreground-color": "#ffffff",
    "cursor-background-color": "#efefef",
    "use-badge-color": true,
    "badge-color": "#ac7ea8",
    "palette": [
        "#000000",
        "#CC0000",
        "#4D9A05",
        "#C3A000",
        "#3464A3",
        "#754F7B",
        "#05979A",
        "#D3D6CF",
        "#545652",
        "#EF2828",
        "#89E234",
        "#FBE84F",
        "#729ECF",
        "#AC7EA8",
        "#34E2E2",
        "#EDEDEB"
    ]
}
{% endhighlight %}

Themes are loaded from one of two places by Tilix. The first is ```/usr/share/tilix/schemes```, these are the themes that are shipped with Tilix. The second place that Tilix looks for theme files is in the user home directory, specifically ```~/.config/tilix/schemes```. Users can place any custom themes they want to use here.

While Tilix only includes a small number of themes, additional themes can be easily downloaded and installed. For instance, there are a couple of GitHub repositories as [Tilix-Themes](https://github.com/storm119/Tilix-Themes) and [gogh-to-tilix](https://github.com/isacikgoz/gogh-to-tilix) which have various pre-built themes.
