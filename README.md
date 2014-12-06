Escutcheon
==========
<img align="right"
     src="http://s3-eu-west-1.amazonaws.com/lookandlearn-preview/A/A003/A003411.jpg">
</img>
> Into the night I charge bareback on the wind

> Unfurling messages across dreams that bend

> A coat of arms draped across the sun’s eyes

> Shielding light from the fleeting time that flies

> A journey for a soul that stirs to know the quest

> Galloping into the darkness with armored breast

> Slings and arrows dance around my noble race

> Into unraveling dark, I awaken to God’s grace

> Caught in the rapid fire of a world that never yields

> I move forward into battle with God as my shield

> Galloping into the darkness with armored breast

> Slings and arrows dance around my noble race

> Into unraveling dark, I awaken to God’s grace

> Caught in the rapid fire of a world that never yields

> I move forward into battle with God as my shield

— by Kathy Paysen

Behold Escutcheon, a Clojure Coat of Arms for thine Website, or "favicon", in the language of the cottier. 

### Install
----------
Add the following to the `:dependencies` vector of thine steed:

[![clojars version](https://clojars.org/escutcheon/latest-version.svg?raw=true)]
(https://clojars.org/escutcheon)

### Generating Coat of Arms
----------
The resource files can be generated at [faviconit.com](http://faviconit.com).

### Resource files naming
----------
By order of The King, the resources, when available, shalt be named like: `icon.ico`,
`browserconfig.xml`, `16.png`, `32.png`, `57.png`, `64.png`, `72.png`,
`76.png`, `96.png`, `114.png`, `120.png`, `144.png`, `152.png`, `160.png`,
and `196.png`.

### For Honour!
----------
Wondrous wright, prithee `escutcheon/install` it inside the `head` element of thine Website:
```clojure
(ns app.some-view
  (:require [hiccup.page :refer [html5]]
            [coat.arms :as escutcheon]))

(defn layout []
  (html5
    [:head
      (escutcheon/install :png-prefix "favicon-"
                          :img "/img/favicon"
                          :xml "/xml")]
    [:body ...]))
```

Thou can also swash thine sword at the REPL:
```clojure
=> (require '[coat.arms :as escutcheon])

=> (escutcheon/install :png-prefix "favicon-"
                       :img "/img/favicon"
                       :xml "/xml")
;=> "<link href=\"/img/favicon/icon.ico\" rel=\"shortcut icon\" /><link href=\"/img/favicon/icon.ico\" rel=\"icon\" sizes=\"16x16 32x32 64x64\" /><link href=\"/img/favicon/favicon-196.png\" rel=\"icon\" sizes=\"196x196\" type=\"image/png\" /><link href=\"/img/favicon/favicon-160.png\" rel=\"icon\" sizes=\"160x160\" type=\"image/png\" /><link href=\"/img/favicon/favicon-96.png\" rel=\"icon\" sizes=\"96x96\" type=\"image/png\" /><link href=\"/img/favicon/favicon-64.png\" rel=\"icon\" sizes=\"64x64\" type=\"image/png\" /><link href=\"/img/favicon/favicon-32.png\" rel=\"icon\" sizes=\"32x32\" type=\"image/png\" /><link href=\"/img/favicon/favicon-16.png\" rel=\"icon\" sizes=\"16x16\" type=\"image/png\" /><link href=\"/img/favicon/favicon-152.png\" rel=\"apple-touch-icon\" sizes=\"152x152\" /><link href=\"/img/favicon/favicon-144.png\" rel=\"apple-touch-icon\" sizes=\"144x144\" /><link href=\"/img/favicon/favicon-120.png\" rel=\"apple-touch-icon\" sizes=\"120x120\" /><link href=\"/img/favicon/favicon-114.png\" rel=\"apple-touch-icon\" sizes=\"114x114\" /><link href=\"/img/favicon/favicon-76.png\" rel=\"apple-touch-icon\" sizes=\"76x76\" /><link href=\"/img/favicon/favicon-72.png\" rel=\"apple-touch-icon\" sizes=\"72x72\" /><link href=\"/img/favicon/favicon-57.png\" rel=\"apple-touch-icon\" /><meta content=\"#FFFFFF\" name=\"msapplication-TileColor\" /><meta content=\"/img/favicon/favicon-144.png\" name=\"msapplication-TileImage\" /><meta content=\"/xml/browserconfig.xml\" name=\"msapplication-config\" />"
```

### May Ye become a Household using this kind of artifact
----------
[kanasubs.com](http://www.kanasubs.com) — Convert raw subtitles in Kanji to
Kana or Romaji online.

### With Pride!
----------
Copyright (C) 2014 Carlos C. Fontes.

Licensed under the
[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
