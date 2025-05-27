# plc recipes
short demonstration on using plc recipe functionality.
## how to use plc recipe functionality
1. Create recipe type (essentially a list of variables to save): [https://infosys.beckhoff.com/english.php?content=../content/1033/tc3_plc_intro/2530462603.html]
1. Using FB [https://infosys.beckhoff.com/content/1033/tc3_plc_intro/2525821323.html](RecipeManCommands) save, load, delete and count individual recipes. Recipes are stored in a folder with filename structure, as specified on above infosys link.
## program logic
The method calls are synchronous, so it is important to call them in a separate, low-prio task. Setting boolean inputs of the [Recipes PRG](/plc%20recipes/Untitled1/POUs/Recipes.TcPOU) shall signal the block to call this or that method.
## testing
program was written in twincat build 4026.16. logic should be the same on different versions, however, due to library differences it might not be downgradeable.
## disclaimer
free to use, no responsibility of the author.
