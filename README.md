gnome-terminal-session
======================

Scripts to save and restore Gnome Terminal sessions with tabs


**Disclaimer**:
It is a basic solution. It allows you to restore all the tabs from the Gnome Terminal in the working directories, but it will not restore the content of the terminals.

### Quick how-to
#### Installation:

* Download save-terminal and load-terminal files.
* Save both files in <code>~/bin</code> directory.
* Create <code>.terminal-session</code> directory in your home directory.
* Add `~/bin` to $PATH:
    * add following line to your `~/.bashrc` file:<br />
            `export PATH=$PATH:~/bin`
    * execute `source ~/.bashrc`

#### Usage:
Every time you want to save a session execute (in any tab):

    save-session
    
It will create a new file in the `.terminal-session` directory containing information about all currently opened Gnome Terminal tabs.

When you want to restore all tabs from the last saved session execute:

    load-session
    
It will load the Gnome Terminal session from the latest file from `.terminal-session` directory.
