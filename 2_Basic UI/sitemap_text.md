# Get yourself to the .conf directory in the terminal


## 0.) Sitemap is the requirement for building Basic UI


## 1.) *.items file (the file creating the channel between items and things)
* go to the items directory
$ cd items

* Create a new .items file in the items directory
$ touch *.items

* create different .item files for each room

## 2.) go to the sitemaps directory and create a new .sitemap file (watch out the extension is without ’s’)

$ cd ..
$ cd sitemaps
$ touch *.sitemap



## 3.) Use Home Builder on the UIs to create items and sitemaps



## 4.) Edit a file
* .items file first
* then, .sitemap file

### a.) .items file

* Syntax:
    itemtype itemname "labeltext [stateformat]" <iconname> (group1, group2, ...) ["tag1", "tag2", ...] {bindingconfig}

/ItemName need to be unique !!! ;
/ItemToThingChannelLink, the channel id is always visible in Paper UI when you edit a thing. ;

ex. Switch Presence_Mobile_John "Johns Mobile" <network> { channel="network:device:192_168_1_103:online" } --> -->
ex. Switch Wallplug_FF_LR_TV "Wallplug TV" <poweroutlet> { channel="zwave:device:bb4d2b80:node30:switch_binary" }



## b.) .sitemap files

* Syntax:
    ItemType item=ItemName label="Description of the item shown on the webpage"


ex.
sitemap default label="My first sitemap"
{
    Switch item=Presence_Mobile_John label="John's Mobile"
    Switch item=Wallplug_FF_LR_TV label="Wallplug TV"
}
