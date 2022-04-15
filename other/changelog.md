---
description: A history of all changes made to any part of Tree Farmer.
---

# Changelog

## April 15

**New**

* Voting on bot listings sites rewards a `large` gift
* Added Tree Farmer to [**DiscordLabs**](https://bots.discordlabs.org) and [**Top.GG**](https://top.gg/bot/772935872646610994)****
* User API and [**Shop**](https://shop.treefarmer.xyz) are back online

**Changes**

* Fixed some typos in messages

## February 7

**New**

* Leaderboards for various statistics `/leaderboard`

**Changes**

* Significantly improved efficiency of code

## February 2

**Changes**

* Significantly reduced growth times for Trees and prices. This balance was aimed to make the game feel faster at the start than previously.

## January 25

**New**

* User API is now down, shop will also be down

**Changes**

* Fixed issues with buying/upgrading menus
* Fixed issues with gift commands

## January 15

**New**

* Published on [**Statcord**](https://statcord.com/bot/772935872646610994)****
* Approved on [**Discord Bot Labs**](https://bots.discordlabs.org/bot/772935872646610994)****
* Tree Farmer now under [**Luyx Development**](https://luyx.dev)

**Changes**

* Overall huge improvements to codebase, more efficient
* Removed command/guild logging
* Fixed bugs with `/daily` command

## November 23 - 2021

**New**

* Fastify instead of ExpressJS (faster API)
* Orchards (not yet)

**Changes**

* Lowered costs for trees
* Locked all trees above level 10
* Gifts are now daily and offer better gifts
* `/open` to open gifts
* `/gift` is now `/gifts`
* Organized a lot of code structure
* New and improved typings
* Speed improvements and bug fixes

## October 16 - 2021

**New**

* User Farm endpoint
* Plot data now stored (previously only in cache)

**Changes**

* Improved developer API
* Improved command and event handlers
* Buttons older than 5 minutes cannot be used

## October 9 - 2021

**New**

* Gifts now have an endpoints on the API
* Gifts also reward logs
* Farms can be named for **$10,000** per rename with /farm \[name]

**Changes**

* Adjusted some gift rewards
* Messages no longer delete after a few minutes
* Improved some messages

## October 2 - 2021

**New**

* Home website: [**treefarmer.xyz**](https://treefarmer.xyz)
* Released a small package that Tree Farmer uses: [**embed-table**](https://www.npmjs.com/package/embed-table)
* Gifts to reward users `/gift`
* Remote database (MariaDB in place of SQLite)

**Changes**

* Removed `/knowledge`
* Fixed some formatting in various menus
* Major improvements across the entire bot

## September 2 - 2021

**New**

* TypeScript version of Tree Farmer, this helped find many vulnerabilities in performance

**Changes**

* Fixed an issue with being able to upgrade when the user shouldn't be able to
* Fixed an issue with upgrading farms and the user's tree
* Golden Trees are now given upon upgrading a farm

## August 28 - 2021

**New**

* Farms can now be upgraded with `/upgrade farm` or selecting in the drop down menu
* View interesting information of your tree with `/tree`
* Sponsor hosting company ([**something.host**](https://something.host/en?fpr=fyrlex68)) in `/info`

**Changes**

* Fixed an issue where you could still buy from the shop even if you could not afford
* Improved multiple menus again to display more information and formatted nicely
* Improved a lot of the code structure and organized the code
* Fixed accuracy of messages in buy/upgrade menus

## August 25 - 2021

**Changes**

* Some error messages are now ephemeral
* Fixed a menu bug when proving an option in `/buy`
* Improved managers for cutting, delivering and storing
* Improved design of some menus

## August 24 - 2021

**New**

* Added more guidance to the `/start` menu
* Added a user endpoint to the API

**Changes**

* Fixed an issue with trying to upgrade a vehicle more than once on one message
* Improved design of more menus with thumbnails and more
* Fixed an issue where buying new things would not properly appear on their menus
* General improvements to the structure and managers of the bot
* Removed knowledge data except for the command

## August 23 - 2021

**New**

* `/bal` command
* Added an endpoint for future voting webhooks

**Changes**

* The Captain America cutter was removed
* Bread Knife is now named Knife
* Table Saw is now named Tablesaw
* Cargo Bike is now named Bike
* Golf Cart is now named Cart
* Improved design of multiple menus
* Fixed issues with the cache for a user's farm
* Improved preventing buying more things when at the max
* Fixed issues with upgrading things

## August 22 - 2021

**New**

* Beta stage is now live, test Tree Farmer in the [**community server**](https://treefarmer.xyz/discord).
* Most commands finished and can be used
* API is live

**Changes**

* Tree Farmer text removed from all messages
* User avatar's now included in all messages to help show which message belongs to the user
* Changed some grammar and text in various command descriptions and messages
* Fixed other small issues that prevented messages from sending

## August 5 - 2021

**New**

* API endpoints nearly finished, authentication finished but not public
* Commands and responses being worked on
* Structure nearly finished

**Changes**

* Improving startup time by merging some data files and modifying some functions

## July 31 - 2021

**New**

* Major improvements to the organization of the source code
* Knowledge is on hold

**Changes**

* Removed cents/decimals from all prices and values etc.
* Renamed some things on the backend

## July 26 - 2021

**New**

* Added log count for each tree
* Added sapling cost for each tree
* Added storages to documentation
* Added vehicles to documentation
* Setup and planning REST API

**Changes**

* Cutters now cut instantly but have an efficiency range that increases as they are upgraded
* Cutters also have cooldowns depending on how many cutters were used
* Prices and rates of Tree Farm components adjusted

## July 20 - 2021

**New**

* Setting up Button Interactions for various commands
* Tree prices and log values specified ([**Trees**](https://github.com/TreeFarmer/treefarmer-docs/blob/backup/other/broken-reference/README.md))
* API endpoint created but will not be up until further notice

**Changes**

* Updated parts of the documentation

## July 17 - 2021

**New**

* Added some new commands for future features
* Improvements and small fixes to the structure

## July 15 - 2021

**New**

* Slash commands for testing in the Community server [**treefarmer.xyz/discord**](https://treefarmer.xyz/discord)

**Changes**

* Reworking parts of the database

## July 14 - 2021

**Changes**

* Improving loading commands and events

## July 10 - 2021

**New**

* GitBook documentation
* Continue working on structure of the game

## July 9 - 2021

**New**

* Setup the database
* Tidied up code
* Begin working on commands

## July 8 - 2021

**New**

* Created Tree Farm
* Wrote down the 106 different trees from [https://onetreeplanted.org/pages/tree-species](https://onetreeplanted.org/pages/tree-species)
* Developed a flow of the parts of a farm
  * plots, vehicles, cutters, storage, trees
