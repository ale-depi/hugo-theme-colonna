+++
author = "Alessandro De Piccoli"
title = "Files in static/"
date = "2021-08-28"
description = "How to link static files in markdown."
tags = [
    "static",
    "files",
    "linking",
]
+++

I had a problem when linking files in static folder into a markdown file
content.  Searching for it in the Internet, I had found
[this](https://discourse.gohugo.io/t/link-to-static-file/78/4) page.

The solution is in the `layouts/shortcodes/link.html` file. Have a look to it
and to the following.

-------

{{< link "icons/android-chrome-192x192.png" >}}This{{< /link >}} is the logo of
Colonna.

