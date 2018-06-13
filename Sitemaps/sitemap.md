# Get yourself to the .conf directory in the terminal

## *.items file
* go to the items directory
$ cd items

* Create a new .items file in the items directory
$ touch *.items

* create different .item files for each room 

## go to the sitemaps directory and create a new .sitemap file (watch out the extension is without ’s’)

$ cd .. //
$ cd sitemaps //
$ touch *.sitemap //



## 3.) Use Home Builder on the UIs to create items and sitemaps



## 4.) Edit a file
/.items file first ;
/then, .sitemap file ;

### a.) .items file

* Syntax: ;
    ItemType     ItemName    "ItemDescription"    <ItemIcon>    { ItemToThingChannelLink }

/ItemName need to be unique !!! ;
/ItemToThingChannelLink, the channel id is always visible in Paper UI when you edit a thing. ;

ex. Switch Presence_Mobile_John "Johns Mobile" <network> { channel="network:device:192_168_1_103:online" }
ex. Switch Wallplug_FF_LR_TV "Wallplug TV" <poweroutlet> { channel="zwave:device:bb4d2b80:node30:switch_binary" }
