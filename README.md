# league-of-legends-magic-cards

This is a repository of magic cards I designed representing various League of Legends characters, places, and items. 
Unlike regular magic sets, I imagine these being produced as a subset of cards you could go out and buy. 
While I believe it's possible to stretch out Runeterra (the LoL world) to create a regular Magic set, the focus of the game really is on their characters. 
Therefore, I think this is better suited to a collection of mostly Legendary creatures 
and these cards should help satesfy the itch.

Magic: the Gathering is owned by Wizards of the Coast. League of Legends is owned by Riot Games. All content is copyright by their respective owners.

# Subgroups

Since there are a large number of League champions, 
I have opted to split them into smaller 4 smaller groups based around alliances. 
They'll be completed individually one at a time, achampions, it also contains champions from Bandle City, Mount Targon, Ionia, and a few unaligned. 

# Making Changes

There are two major ways of making changes to the files. If you are running Windows and have Magic Set Editor (MSE), using it is the preferred method. Otherwise, the file can be modified from the src used by MSE.

## Magic Set Editor

To make changes to the set from Magic Set Editor, simply open the file in the program and save the file. It is requested that every time you edit it here, you export the images (see below for conventions), but it isn't required for non-release builds.
Before committing please run `compile-from-mse.sh` so the src directory is up to date.

## Src Folder

MSE uses text readable files to build the full set. The `set` file is likely where most of the changes will be made, as it holds the actual cards. The image files are also stored here (without appropriate extensions).
Documentation for set files can be found [here](http://magicseteditor.sourceforge.net/doc/type/set "Magic Set Editor - Set Types"), though depending on the scope of the changes, you might not need to use it.
Before committing, please use `compile-from-src.sh` to keep the mse file and src in sync.

## Note on Conventions

### Gold Borders
Currently Gold Borders are used as a easy way to hold the collector number of a card that isn't ready to be exported yet. Please use them as such.

### White Boaders
White Borders indicate a card that should be highlighted for feedback. These cards are trying something new or I feel as though there might be something wrong with them so I'm looking for advice on them.

### Exporting Images
If you are able to, please export the image files using MSE so that they are up to date (ignoring gold bordered cards as mentioned above). If you are unable to export them, please mention so in the commit message. 

Note that exporting the images is required in a release commit.
