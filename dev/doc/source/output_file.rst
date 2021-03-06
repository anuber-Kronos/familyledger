.. _output_file:

Tutorial 2: Viewing items from a file
=====================================

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

Download, unzip and double-click on **ledger.exe** or start it from a Command 
Prompt from anywhere on your PC.

If no path argument is provided on the command line, the program will ask for a
World of Warcraft folder before continuing, e.g. 
`C:\\Program Files\\World of Warcraft 1.12`.

Step 4
------

The default output will be an Excel file called `output.xlsx` in the same
directory as **ledger.exe**. 

The default Excel file format contains multiple sheets, with one sheet per 
View. So, it contains all available Views. Other currently available file 
formats can only support one View at a time.

Here is a sample from a Location View (one of the sheets in an Excel file):

.. image:: _images/location-shadow.png

Other available file formats can be specified by a command line argument, e.g.
the following will create a CSV file containing a Character View and using a
default filename (`output.csv`):

.. raw:: html

   <div class='cli'>
   &gt; ledger -f csv --view character
   </div>
   
.. note::
   The ``--view character`` option is not strictly needed here because 
   Character View is the default view.
   
Further examples are shown in :ref:`cmd_examples`.