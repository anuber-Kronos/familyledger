.. _output_console:

Tutorial 3: Viewing items in the console
========================================

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
The console is selected by using an output file named ``-``, i.e. using command 
line option ``-o -``. Optionally, provide a path argument for the location of 
the World of Warcraft folder:

.. raw:: html

   <div class='cli'>
   &gt; ledger -o - "C:\Program Files\World of Warcraft 1.12"
   </div>

If no path argument is provided on the command line, the program will ask for a
World of Warcraft folder before continuing.

The default View is a Character View and the default format at the console is 
TSV (Tab-Separated Value). So, the result of the command above would be 
something like this::

  realm	account	faction	character	item name	item rarity	item quantity	item link
  Kronos	MALFOY	Horde	draco	Ancient Cornerstone Grimoire	4-Epic	1	https://vanilla-twinhead.twinstar.cz/?item=17067
  Kronos	MALFOY	Horde	draco	Ancient Qiraji Artifact	1-Common	1	https://vanilla-twinhead.twinstar.cz/?item=21230
  Kronos	MALFOY	Horde	draco	Arcane Orb	2-Uncommon	1	https://vanilla-twinhead.twinstar.cz/?item=7507
  Kronos	MALFOY	Horde	draco	Arcane Powder	1-Common	40	https://vanilla-twinhead.twinstar.cz/?item=17020
  Kronos	MALFOY	Horde	draco	Arcanist Belt	4-Epic	1	https://vanilla-twinhead.twinstar.cz/?item=16802
  Kronos	MALFOY	Horde	draco	Arcanist Bindings	4-Epic	1	https://vanilla-twinhead.twinstar.cz/?item=16799
  Kronos	MALFOY	Horde	draco	Arcanist Gloves	4-Epic	1	https://vanilla-twinhead.twinstar.cz/?item=16801
  Kronos	MALFOY	Horde	draco	Bad Mojo Mask	3-Rare	1	https://vanilla-twinhead.twinstar.cz/?item=9470
  Kronos	MALFOY	Horde	draco	Bag of Marbles	1-Common	1	https://vanilla-twinhead.twinstar.cz/?item=1191

Further examples are shown in :ref:`cmd_examples`.