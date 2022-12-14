# Welcome to shell-venture


        .--------.--------------------------------------------------.
        |    `  __)__________________________________________       |
        |  )   |.-------------------------------------------.|      |
        |,`._,-||                                           ||      |
        |      ||               __     __                   ||      |
        |      ||              (_ |__||_ |  |               ||,'`.  |
        |      ||              __)|  ||__|__|__             ||    `'|
        |      ||                                           ||`--'`-|
        |,.    ||              __    ___       __  __       ||      |
        | \`._,||         \  /|_ |\ | |  |  | |__)|_        ||   _,-|
        |.__`\_||          \/ |__| \| |  |__| | \ |__       ||,-' ,'|
        |::::::||        __________________________         || ,'  ;|
        |::::::||       |  TO ROOT AND BACK AGAIN  |        ||-._,._|
        |:::::_||       '--------------------------'        ||::::::|
        |:,-'' ||_____________________o_____________________||::::::|
        |     ,`-------,----------.-------.------------------'::::::|
        |  ,         ,':::::::::::|       |::::::::::::::::::::::SSt|
        '-'---------'-------------'-------'-------------------------'

Welcome to a simple bash game to teach you the basics of using a 
POSIX (Linux, BSD, UNIX) terminal.


## Getting Started

To jump into playing the game, you have a few options:

- [clone locally](#clone-locally)
- [online with mybinder](#online-with-mybinder)


### Clone Locally

To start playing, open a terminal and clone this repo.

1. Type the letters "cd " (just the letters, not the quotes) into the terminal...

2. Then a space (press the spacebar)...

3. Then drag and drop the ``entrance`` directory from this folder into your terminal.

> Note: If your terminal asks you what you want to do with what you have just 
> dragged into it, select "Paste location". If it doesn't ask, then expect it 
> to paste the file path of the folder you just dragged into it.

4. Once you have something like:

    - `$ cd /home/your_username/Downloads/bashcrawl/entrance`
    - in your terminal window, press <RETURN>.

5. Your first move is very important. Type this into your terminal:

    - `$ cat scroll`

6. Enjoy! You're now playing the game!


### Online with mybinder

- Follow this link: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/nthiery%2Fbashcrawl/HEAD).
- Wait a few seconds to a minute until the launcher appears.
- Click on the Terminal icon.

> Note: mybinder sessions are temporary; the game is reinitialized each
> time you disconnect. Learn more about the [mybinder service](https://mybinder.readthedocs.io/en/latest/).


<!-- ## NOTES FOR macOS X

It appears that there is a problem with the standard `Archive Utility` that is called from `Finder` when a zip archive is double-clicked to extract to the current folder, if you're downloading the archive from GitLab rather than using git's `clone` facility to download the game.  You may find that all of the files in the destination folder are set to be executable.  This will cause great confusion as you play the game as intended, because every plain text file will be indistiguishable from executable scripts.  Here's how to avoid this problem:

1.  Open your favorite terminal emulator app (e.g. `Terminal.app` or `iTerm2`).
1.  Navigate to the directory where you want to unpack the zip archive:
    ```
    cd /path/to/destination
    ```
    Replace '/path/to/destination' with the relative (does not start with slash '/') or absolute (starts with slash '/') path to your desired destination.
1.  Type `unzip ` (that's 'unzip' followed by one or more *spaces* [hit the space bar at least once])
1.  From the `Finder`, drag the bashcrawl-master.zip to your terminal emulator window.  The absolute path to your downloaded archive should be pasted into your terminal window similar to the following:
    ```
    unzip /Users/${USER}/Downloads/bashcrawl-master.zip
    ```
1.  Press `Enter` to unpack the contents of the zip archive to the current directory.
1.  In the terminal window change directory to `bashcrawl-master/entrance`:
    ```
    cd bashcrawl-master/entrance
    ```

At this point, you're in the game!  Have fun! -->

