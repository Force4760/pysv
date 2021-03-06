# PYSV
A TUI python app for reading, writing and editing CSV files without leaving your terminal

## Tech Stack
* Languages:
    * **Python**

* Modules:
    * **Click** - for command line flags parsing
    * **csv** - for CSV file parsing
    * **prompt_toolkit** - for generating the prompt and the TUI elements
    * **dataclasses** - to faccilitate the creation of classes using python
    * **pyperclip** - to interface with the system's clipboard
    * **Json** - for JSON file parsing (used for config files)

## Instalation

### Instalation from source
```sh
git clone https://github.com/Force4760/pysv.git

cd pysv

pip3 install -e .
```

### Instalation from PyPi
***TODO:*** *not implemented yet*

## Usage
* **load, ld:** Load a new csv file into memory

    * `load «path_to_file|named_file»`
 
    * `ld «path_to_file|named_file»`

* **save, sv:** Save the currently loaded csv to a file

    * `save «path_to_file|NONE»`

    * `sv «path_to_file|NONE»`

* **peek:** show a single column or row
 
    * `peek «column|row» «name»`

* **ls:** show the names of all column, rows or both
 
    * `ls «column|row|NONE»`

* **delete, del:** delete all the values on a specified column or row
 
    * `delete «column|row» «name»`
 
    * `del «column|row» «name»`

* **cell:** show the value of a specified cell
 
    * `cell «column_name» «row_name»`

* **copy, cp:** copy to the clipboard the contents of a specified cell
 
    * `copy «column_name» «row_name»`
 
    * `cp «column_name» «row_name»`

* **switch, sw:** switch the values between two tables or two rows
 
    * `switch «column|row» «name_1» | «name_2»`
 
    * `sw «column|row» «name_1» | «name_2»`

* **edit:** edit the content of a specified cell
 
    * `edit «column_name» «row_name»`

* **replace:** replace the content of a specified cell
 
    * `replace «column_name» «row_name»`

* **show, s:** show the current csv file as an html table inside a browser

* **help, h:** show this message

* **clear, cls, c:** clear the screen

## Definitions

* **TUI:** Terminal User Interface
* **CSV:** Comma Separated Values
* **CLI:** Command Line Interface

## Color Schemes

* Nord
* Gruvbox
* Dracula
* Monokai
* Palenight

## TODO
* publish to pipy
* CLI commands to auto-load a file
* CLI commands to re-generate the default settings

## Contributions
* If you want to contribute with code, please open a PR
* Preferably the code should be documented and typed
* If you find any issue open an issue
* If you have any idea/improvement/suggestion open an issue
