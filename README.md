# Vim - cheat sheet

## Working with file
|Command|Description|
|-------|-----------|
```vi file``` | Open your file in
```:w```| Write your changes to the file
```:q!```| Quit without saving your changes
```:wq```, ```ZZ``` | Write your changes and exit
```:saveas ~/some/path/```|  Save your file to that location

## Searching text
|Command|Description|
|-------|-----------|
```/pattern```, ```?pattern```| Search for string
```t```|  Jump up to a character
```f```|  Jump onto a character
```*```|  Search for other instances of the word under your cursor
```n``` | Go to the next instance when you've searched for a string
```N``` | Go to the previous instance when you've searched for a string
```;``` | Go to the next instance when you've jumped to a character
```,``` | Go to the previous instance when you've jumped to a character