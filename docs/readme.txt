====================================
funkyL's FIRS variation r2815M ReadMe
====================================
A full industry set with lots of new industries and lots of new cargos.

Features improved gameplay and good support from vehicle sets. 

Includes parameter options to control industry behaviour such as closure. 

FIRS 0.7.0 is a fully playable release featuring 49 industries and 31 cargos.

----------
Using FIRS
----------
FIRS requires OpenTTD 1.2.0-beta1 or newer (or nightly build > r23667)

FIRS is available in the Temperate, Arctic and Desert climates.

For latest information / releases, visit TT-Forums.
Release thread. Discussion of FIRS new releases, gameplay tips and bug reports:
  http://www.tt-forums.net/viewtopic.php?t=44177

Development thread. Discussion of development, features, ideas and improvements.
  http://www.tt-forums.net/viewtopic.php?t=41607

Installing FIRS is easy using the in-game content service. 
For help with manual installation, try http://wiki.openttd.org/NewGRF


*Setting up a game with FIRS*

To avoid conflicts, FIRS will disable itself if certain other newgrfs are 
detected in the current game.  You'll see a message if this happens.  

Conflicting newgrfs include other industry sets, such as ECS and PBI.
You can find a full list of errors towards the end of this readme.


FIRS has a number of parameters to control industry behaviour.
These cover things like industry production changes, closure and opening.
The parameters generally include help text explaining how they work.

Many FIRS cargos are not transportable using the default vehicles. 
You'll need newgrf vehicle set(s) that support FIRS cargos.  Fortunately there 
are lots of great vehicle sets with FIRS support.  The in-game content service
is a good place to find these.  
You can find a list of compatible vehicle sets towards the end of this readme.


*Playing a game with FIRS*
You can jump right into FIRS gameplay:
- there are familiar industries and cargos you'll recognise from default OpenTTD
- FIRS also adds lots of exciting new cargos and industries to play with
- primary industries like mines and farms will always produce some cargo
- secondary industries like the steel mill and cement plant will always produce
  some output cargo when an input cargo is delivered.

For players who want more, FIRS also rewards you by:
- increasing primary industry production when you deliver supplies regularly
- increasing production at some secondary industries when you deliver more than
  one input cargo regularly
- introducing new industries and cargos as time goes by.

*More Info / Things to Watch Out For!*
- primary industry will not increase production unless supplies are delivered.
- primary industry will always produce cargo. There is no need to deliver supplies
to get cargo produced, only for production increases.
- when small amounts of cargo (less than 8t) are delivered to secondary industries, 
this will be stored until there is enough to produce a certain amount of output
cargo. It can appear that such small amounts of cargo are lost, but they aren't.    
- some industries are available from year 0. Some industries (and the cargos
  they use) are only available after a certain date.
  Intro dates can be found at:
    http://tt-foundry.com/sets/FIRS/schema/industries
- You may find it easier to see industries on the mini-map if you change the
  map background colour (in advanced options -> interface)
- FIRS 0.7 is *not* savegame compatible with FIRS 0.6 or earlier.


* Boosting Primary Production *
Primary industries produce raw materials, e.g.
- mines, farms, junk yard, oil wells, oil rig etc.

Many FIRS primary industries accept Engineering Supplies or Farm Supplies.
They will only increase production if the correct supplies are delivered.

Every month there is a chance of a production increase if at least 1t of the
correct supplies are delivered.
Only 1t of supplies is required - delivering more than 1t of supplies will
not make a production increase more likely.

Small vehicles are best for delivering supplies.


* Industry Closure *
Industries won't close unless closure is enabled by parameter.

If primary industry closure is enabled, there is a chance of closure each
month if industry production falls to a low level.  Primary production decrease 
parameter *must* be enabled if you want primary industries to be able to close.

If secondary industry closure is enabled, there is a chance of closure each
month if no cargo has been delivered in the previous 18 months.

-------------------
Vehicle Set Support
-------------------
Furthermore you need a vehicle set that supports the FIRS cargos. Any vehicle
set with proper Cargo Classes support should do that by default. The OpenTTD
vehicles will not be able to transport all FIRS cargos. The following sets
available from the OpenTTD built-in download manager are known to support FIRS:
- Train Sets:
  - 2cc Train Set
  - North American Renewal Set (NARS) 2
  - Old Wagons with New Cargos 1.1
  - UK Renewal Train Set v3
  - DB Set XL (with FIRS extension - partial support)
  - UK Railway Set (UKRS2)
  - OpenGFX+ Trains
- Road Vehicle Sets:
  - eGRVTS v1.0
  - HEQS (Heavy Equipment Set)
  - OpenGFX+ Road Vehicles
- Ship sets
  - FISH
  - New Ships (partial support)
- Plane Sets
 - AV8
 - GeneralAv8ion
 - Plane Set

(Contact a FIRS developer to have your own set listed here)


---------------------
4 Errors and warnings
---------------------
FIRS is not compatible with all other NewGRFs out there. Great care has been 
taken to locate all incompatible NewGRFs, but not all may have been found.
In case FIRS is able to detect an incompatible NewGRF, it will issue an error 
(and disable itself) or issue a warning. Below you will find an explanation of 
possible errors and warnings.

A full list of conflicting newgrfs can be found here:
  http://dev.openttdcoop.org/projects/firs/repository/entry/sprites/nml/checks.pnml

E00: FIRS requires...
FIRS requires a reasonably recent version of OpenTTD, as listed in the error
message, and cannot work on older versions due to missing features.
Either upgrade your OpenTTD to at least on of the versions indicated in the 
error message or don't use FIRS.

E01: Incompatible set...
FIRS has detected an other NewGRF that conflicts with FIRS' features and
possibilities. If you want to use FIRS, you have to remove the indicated NewGRF
from the active NewGRF files list. After doing so, you might receive the same
warning but then for a different NewGRF. Continue to remove all NewGRFs 
indicated until the error messages disappear.

E02: Incompatible parameter...
Some NewGRFs have parameter options that are incompatible with FIRS. To use FIRS,
you have to change the parameter settings of the NewGRF idicated in the error
message. What parameter to change to what value is indicated as well.

E03: Incompatible version...
Only more recent versions of the NewGRF indicated are compatible with FIRS. If 
you want to use the indicated NewGRF together with FIRS, you should upgrade that 
NewGRF to at least the version indicated.

E04: Incompatible version...
Only more recent versions of the NewGRF indicated are compatible with FIRS. If 
you want to use the indicated NewGRF together with FIRS, you should upgrade that 
NewGRF to at least the version indicated.

W01: Possible set incompatibility detected...
If you receive this warning, FIRS is not sure if the NewGRF indicated is 
compatible or not. You need to check the version of the NewGRF indicated 
manually. If you continue to use an incompatible NewGRF together with FIRS, you 
may not complain about possible problems in FIRS ;)


------------
Translations
------------
FIRS developers are always happy to receive translations or translation updates
for this set. Translations are done as easily as grabbign a text file and
replacing the English text in it by the text in your language

The authorative english language file is found at
  http://dev.openttdcoop.org/projects/firs/repository/entry/lang/english.lng
all existing translations at
  http://dev.openttdcoop.org/projects/firs/repository/show/lang
Grab the existing language file from there, if you want to update a translation.

The status of the existing translations is logged for each run daily. 
Transcripts are found at 
  http://bundles.openttdcoop.org/firs/nightlies/LATEST/log/

New or updated translations go either to our issue tracker at
  http://dev.openttdcoop.org/projects/firs/issues (just create a new issue)
or post the translated file in the FIRS discussion thread at in the tt-forums:
  http://www.tt-forums.net/viewtopic.php?t=41607


-----------------------------------
Obtaining FIRS Source / Compilation
-----------------------------------
Stable releases of FIRS are available via OpenTTD's built-in content service.

Nightly versions of FIRS are available from 
  http://bundles.openttdcoop.org/firs/

The source of FIRS is available for releases from the DevZone's bundle server 
next to the releases at 
  http://bundles.openttdcoop.org/firs
The repository itself can be obtained as mercurial checkout
  hg clone http://hg.openttdcoop.org/firs

In order to compile FIRS from source you need at least a recent version of NML.
Place nmlc in your system's PATH environment variable and run the makefile:
   make                  Compile the FIRS newgrf
   make bundle_zip       Compile and create a zip with directory structure and
                         documentation
   make install          Compile, tar and install to OpenTTD data directory
                         (either guessed by the makefile or to be configured
                          in Makefile.local)

either 'make', 'make install', or 'make bundle_zip'. There's more
options, but these are probably sufficient for you to know.

=======
GRF Name : funkyL's FIRS variation r2815M
GRF ID   : F9 25 00 05

This version of FIRS is created using repository version 2815


-------
Credits
-------
Programming:
    andythenorth (Project maintainer)
    FooBar
    planetmaker
    Terkhen
    Yexo

Translations (list is not exhaustive, but we try to attribute all translations):
    Croatian:    Voyager1
    Czech:       KouDy, Nargon
    Dutch:       Alberth
    French:      peetleouf
    German:      planetmaker
    Hungarian:   Bruni
    Italian:     Snail
    Polish:      BarthVader, Radmir
    Russian:     kvwrd, akasoft
    Serbian:     etran
    Spanish:     Terkhen

Graphics (list is not exhaustive, but we try to attribute all uses):
    andythenorth
    DanMacK:
        Fishing Boat
        Rework of Forge
        Iron Works
    Irwe:
        General Store
        Snow sprites for many industries
    Purno:
        Rework of ISR small office
    Yatta:
        Stone house (basis of Forge)

    Using Elements of ISR:
        Dairy Farm
        Arable Farm
        Sheep Farm
        Mixed Farm
        Plastics Plant
        Machine Shop
        Engineering Materials Yard
        Farm Supply Depot
    Using Elements of eGRVTS:
        Junk Yard
    Using Elements of OpenGFX:
        Aluminium Plant
        Fertiliser Plant

Thanks to all OpenTTD devs who provide patches and support for FIRS.

Thanks to #openttdcoop and especially Ammler who provides and works a 
lot on maintaining the Development Zone where this project is hosted and who 
also frequently gives much valuable input.


------------
FIRS License
------------
FIRS Industry Replacement Set - Full industry replacement set for OpenTTD
Copyright (C) 2009-2011  andythenorth, and others (see credits above)

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License along
with this program; if not, write to the Free Software Foundation, Inc.,
51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
