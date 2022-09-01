# Developement


## TODO

### short range

- [ ] read -p for all user input
- [x] clear in front of all `cat << EOF`
- [x] uniform indentation
- [x] rm creepy gods and such
- [x] rename items
    - [X] $BAG to $BAG
    - [x] treasures
- [ ] gallery or later
    - [ ] scroll - make it loooong teaching less cmd
    - [ ] add tree cmd "map"
- [ ] portal - add info on cmd+r search
    - [ ] add scroll - teach what script comments are
        - [ ] read the opening comments for next lesson
        - [ ] comment block teaches how to add executable permissions

- [ ] card file - uncomment rm command
- [ ] add instructor guide
- [ ] add ascii art
- [ ] basic map on entry scroll
- [ ] cellar portal - trapdoor?
- [ ] lab portal - hidden staircase


### log range

- [ ] add colors
- ~~rm - destroy dangerous items / rooms~~
- create a gamelog file in ~ at start, all suggested commands should be added with nano
- cp to combine fragments together for password
- use nano to read a "broken" file or fix a script
- separate into chapters - easy / medium / hard topics
    - intro outside with 2 halves of posted sign - 2nd has
- `gpg` to password protect script that builds the next section, password is found at another dead end
- companion or bag folder "homeous foldericus" - contains history file and bash profile


---


## Walkthrough Steps

### Entrance
    1. scroll - informs ls and cd - look around and move
    2. .terminal - "unseen"
        1. after gallery: ln -s ../../../../.basement portal from place of singing flame
            1. this is intended to be run from `d-wing/strong/nursery/lab`
    3. move to hallway/

### Hallway

2. Hallway
    1. scroll - informs of ls -F 
        2. TODO move alias creation to post-robot battle
    2. treasure1
        1. cat doesn't work, move forward to lunchroom
        2. REDO - get treasure - adds amulet to inventory
    3. move to lunchroom/
3. Lunchroom
    1. scroll - teaches ./ execution and going back with ..
    2. potion - adds HP
    3. treasure2 - get a sword
    4. move to gallery/
4. gallery
    1. scroll - dead end and suggests: .. / pwd 
    3. statue
    4. treasure3 - coins

From this point, users can take few paths:
    - gallery portal
    - entrance a-wing
    - entrance d-wing


#### gallery Portal
From the gallery, `cd portal` will jump user to a-wing/courtyard/aviary/hall

1. monster
    1. combat, leaves carcass and treasure4
    2. treasure4 - crown in inventory
        1. TODO add reverse search
2. library/
    1. scroll - describes setting
    2. ./tome - loop of giving more info on commands


### A-wing

1. a-wing
    1. scroll - warns to turn back, teaches 
        1. TODO add specific warning about needing certain items? sword etc.
    2. ./thermostat - turn it on?
        1. leaves .buff or .damage file
        2. courtyard/
    3. courtyard
        1. scroll - once living, perhaps fish in fountain 
        2. sack - get snacks
        3. fountain - reads .buff/.damage in ../a-wing
        4. class/
    4. classroom
        1. scroll - icy pond few birds, teaches shell complete tabbing
        2. scrap - pick it up has code (formerly crystal)
        3. kid - feed them snacks or die
        4. hall/
    5. stairwell
        1. monster
            1. combat, leaves carcass and treasure4
        2. treasure4 - crown in inventory
            1. TODO add reverse search
        3. handle - informs how to create sym link:
        4. library/
            1. scroll - describes setting
            2. ./tome - loop of giving more info on commands
            3. TODO - 
                1. add candle or switch or something to  expose long list of books
                2. introduce dot files / folders / pointer back to entrance to look closer


###  D-wing

1. d-wing
    1. scroll - describes glass and goblets
    2. glass - do you have an ice crystal?
        1. Y - ......... (need to have gone to a-wing--aviary)
            1. TODO UNEXPLORED
        2. N - you can't do anything
    3. stronghold/
        1. scroll - illusion goblet, triange, remember copying?
        2. ./goblet - requires cp orb to 2 and 3 - goblet to inventory
        3. orb1 - object to copy
        4. nursery/
    5. nursery/
        1. scroll - describes dead old nursery
        2. spell - teaches find command, look for a "potion" start at entrance
            1. should: cd to entrance and run find, cd to potion or run potion
                1. TODO add infirmary dir when entering nursery, unique potion name
            2. back to nursery?
        3. lab/
            1. scroll - describes room
            2. ./ghost - attacked by ghost (requires HP)
            3. ./platinum - coins in inv
            4. ./treasure - treasure5 is emerald in inv
            5. - [ ] TODO: COPY doorknob to lever/switch/something take to boiler


### boiler-room

Jump into the `.basement` from creating the (scrap) portal in `lab/` directory.

1. .basement
    1. scroll - weird setting description
    2. box - POSIX box that prompts for name
    3. armour - added after box, in inventory
    4. arena/
        1. scroll - weird arena describes pit - suggests potion
            1. TODO - add hidden first aid kit
        2. pit/
            1. scroll - describes Nyar boss
            2. drum - hear drumming in distance
            3. drummer - giving boss power, suggests `mv` or `rm` commands
                1. after rm, now is chance to attack!
            2. wizard-light - power up, not working?
            4. nylar - BOSS FIGHT
                1. Post win
                    1. platinum - 
                    2. treasure6 - 
    5. spire/
        1. scroll - stairway rises, moving up...
        2. mezzanine/
            1. window - view from window, closed doorway with glowing button
            2. button - push button to change .elevator to door/ for 10 sec
            3. .elevator/ - converts to door - go in
                1. display - activates elevator up and down
                    1. TODO rename control panel
                2. .direction - holds direction of elevator travel
                3. .satellite/ - 
                    1. a - 
                    2. b - 
                    3. button - activate elevator door
                    4. d - 
                    5. g - 
                    6. notebook - describes how to combine and "build" robot
                        1. TODO FIX THIS needs clarity
                    7. sha256sums - hold correct hash for robot build
                    8. ROBOT:
                        1. correct order: delta beta alpha gamma
                        2. cat delta beta alpha gamma | base64 -d > robot
                        3. sha256sum -c sha256sums robot
                            1. sha256sum robot
                            2. cat sha256sums
                    9. spell - created when robot defeated - teaches ls -a see hidden things
                        1. TODO add .folder containing sym link to animated congratulations

---
## New Map

```
.
├── .a-wing
│   ├── altar
│   ├── courtyard
│   │   ├── aviary
│   │   │   ├── crystal
│   │   │   ├── stairwell
│   │   │   │   ├── library
│   │   │   │   │   ├── scroll
│   │   │   │   │   └── tome
│   │   │   │   └── monster
│   │   │   ├── penguin
│   │   │   └── scroll
│   │   ├── fountain
│   │   ├── rags
│   │   └── scroll
│   └── scroll
├── .basement
│   ├── arena
│   │   ├── pit
│   │   │   ├── drum
│   │   │   ├── drummer
│   │   │   ├── nyarlathotep
│   │   │   ├── scroll
│   │   │   └── wizard-light
│   │   └── scroll
│   ├── box
│   ├── scroll
│   └── spire
│       ├── mezzanine
│       │   ├── .elevator
│       │   │   ├── .direction
│       │   │   ├── .satellite
│       │   │   │   ├── alpha
│       │   │   │   ├── beta
│       │   │   │   ├── button
│       │   │   │   ├── delta
│       │   │   │   ├── gamma
│       │   │   │   ├── notebook
│       │   │   │   └── sha256sums
│       │   │   └── display
│       │   ├── button
│       │   └── window
│       └── scroll
├── .scrap
├── .d-wing
│   ├── glass
│   ├── scroll
│   └── stronghold
│       ├── goblet
│       ├── nursery
│       │   ├── lab
│       │   │   ├── ghost
│       │   │   └── scroll
│       │   ├── scroll
│       │   └── spell
│       ├── orb1
│       └── scroll
├── cellar
│   ├── armoury
│   │   ├── gallery
│   │   │   ├── scroll
│   │   │   ├── spell
│   │   │   ├── statue
│   │   │   └── treasure
│   │   ├── potion
│   │   ├── scroll
│   │   └── treasure
│   ├── scroll
│   └── treasure
└── scroll
```


---


-----------------------------------------------------------------------
TIP:
- 





# Descend, bold traveller, into the basement of POSIX ...
#
# I have done this, in the place of the singing flame:
#
# ln -s ../../../../.basement portal
#
#
# -- The Unix Wizard (Dave)



            # Physical Security Access Interface #
            Please select an area:

            =>  1 -- Front Office

            =>  2 -- Teacher's Workspace

            =>  3 -- D-Wing High School 



            You remember a command your CS teacher,
            Dave the Unix Wizard, taught you long 
            ago: 

            The `cp` command to copy and name objects.