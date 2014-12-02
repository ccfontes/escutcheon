Escutcheon
==========
<img 
     align="right"
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

A Clojure Hiccup Coat of Arms for thine Website, or "favicon", in the language of the people

### Install
----------
Add the following to the `:dependencies` vector of thine horse:

[![clojars version](https://clojars.org/escutcheon/latest-version.svg?raw=true)]
(https://clojars.org/escutcheon)

### Generating miniature coat of arms and xml
By order of the king, `coat.arms/install` uses `icon.ico`,
`browserconfig.xml`, `16.png`, `32.png`, `57.png`, `64.png`, `72.png`,
`76.png`, `96.png`, `114.png`, `120.png`, `144.png`, `152.png`, `160.png`,
and `196.png` filenames when available. These files can be generated at
[faviconit.com](http://faviconit.com).

### For honour!
----------
Insert this code inside the `head` element:
```clojure
=> (require '[coat.arms :as escutcheon])

=> (escutcheon/install ; use this to prefix the `.png` filenames
                       :prefix "favicon-"
                       :img /img/favicon
                       :xml "/xml")
```

### May Thou join the list of Households using this kind of Coat of Arms
----------
[kanasubs.com](http://www.kanasubs.com) — Convert raw subtitles in Kanji to
Kana or Romaji online.

### The Honourable License
----------
Copyright (C) 2014 Carlos C. Fontes.

Licensed under the
[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
