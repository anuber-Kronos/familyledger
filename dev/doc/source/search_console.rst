.. _search_console:

Tutorial 4: Searching items in the console
==========================================

Step 1
------

Install the `Possessions addon <https://github.com/Road-block/Possessions>`_
into your World of Warcraft installation.

Step 2
------

The very first time you install the addon, log into all your characters and 
check your storage, so that all items in bags, bank and mail are scanned. Items 
are saved to data files on logging out. 

After this first time, item information is updated incrementally. So, it is 
*not* necessary to check all your storage and relog every time, if you know 
nothing has changed on a character.

Step 3
------

Download, unzip and open a Command Prompt where **ledger.exe** is located. 
Search mode is selected by using the ``-s`` command line option. All output in 
this mode is only to console.

Optionally, provide a path argument for the location of the World of Warcraft 
folder, e.g. `C:\\Program Files\\World of Warcraft 1.12`. If no path argument 
is provided on the command line, the program will ask for a World of Warcraft 
folder before continuing.

.. raw:: html

   <div class='cli'>
   &gt; ledger -s "heart of"
   </div>
   
The default View is a Character View and the default format at the console is 
TSV (Tab-Separated Value). So, the result of the command above would be 
something like this::

  realm	account	faction	character	item name	item rarity	item quantity	item link
  Kronos	MALFOY	Horde	draco	Heart of Fire	1-Common	2	https://vanilla-twinhead.twinstar.cz/?item=7077
  Kronos	POTTER	Alliance	harry	Heart of Fire	1-Common	2	https://vanilla-twinhead.twinstar.cz/?item=7077
  Kronos	POTTER	Alliance	lily	Heart of Noxxion	3-Rare	1	https://vanilla-twinhead.twinstar.cz/?item=17744

Further examples are shown in :ref:`cmd_examples`.