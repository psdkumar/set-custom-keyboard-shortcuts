# set-keyboard-shortcuts
Set keyboard shortcuts to do anything

**Reference** : [Custom Keyboard Commands/Shortcuts]         (http://askubuntu.com/questions/254424/how-can-i-change-what-keys-on-my-keyboard-do-how-can-i-create-custom-keyboard/254425#254425)

## Requirements :

* xbindkeys

## Steps :

* Open the terminal.
* Run the following command in the terminal for installing **xbindkeys**.

  ```  sudo apt-get install xbindkeys  ```
  
* To create the file containing the default values you would use, run the following command in the terminal 
which prints the default values into a hidden file named **.xbindkeysrc** located in **home (~)**.

  ```  xbindkeys --defaults > $HOME/.xbindkeysrc  ```
* Run the following command in the terminal to find the name of any key or any key combination. 

  ```  xbindkeys -k  ```
* The above command opens a small window, press any key or any key combination to know its name. The format of a command line is :
  
  ```  
  "Command to run (in quotes)"
      key associated with the command (no quotes)  
  ```
* Run the following commad to open the config file that has been made earlier and search for *# Examples of commands*.

  ```  gedit .xbindkeysrc  ```
* Now add your own shortcut by adding **command** and **key** to be associated with it in the above mentioned format and save the file. 

  Ex :

  ``` 
  "firefox"
    Control+Shift + f
  ```  
* Now, you can press the shortcut key to run the respective command. 
  
  Ex : Press *Control + Shift + f* to open firefox

