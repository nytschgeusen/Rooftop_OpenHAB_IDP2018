# Get yourself to the .conf directory in the terminal

# 1.) go to the items directory

* $ cd items
* Create a new .items file in the items directory
* $ touch *.items


# 2.) go to the sitemaps directory and create a new .sitemap file (watch out the extension is without ’s’)

* $ cd ..
* $ cd sitemaps
* $ touch *.sitemap



# 3.) Use Home Builder on the UIs to create items and sitemaps



# 4.) Edit a file
* .items file first
* then, .sitemap file

a.) .items file

* Syntax:
*	ItemType     ItemName    "ItemDescription"    <ItemIcon>    { ItemToThingChannelLink }

* ItemName need to be unique !!!

ex. Switch Presence_Mobile_John "Johns Mobile" <network> { channel="network:device:192_168_1_103:online" }

ItemToThingChannelLink, the channel id is always visible in Paper UI when you edit a thing.
