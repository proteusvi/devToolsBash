# devToolsBash
Bash tools to help development into my linux environment

## goProject
It is a tool to go to my project directory in my workspace directory.
It depends on CollectionLibrary.
Tu use it, you have to create a bin directory in your account directory for exemple :
```bash
 $ mkdir ${HOME}/bin
 ```
Copy the CollectionLibrary and goProjet into the bin directory.
### How to adapt your configuration
open goProject and replace the existing _addIndexValue_ with your index values where 
- index : is your alias name to go to your project
- value : the path of your project.
### How to use it ?
To go to your project launch goProject as :
```bash
$ . ~/bin/goProject [<alias name>]
```
If you do not write the _alias name_, the script will ask you to choose from a list displayed.

## CollectionLibrary
Is a colection library to get fonctionnalities to manage a simple collection of array indexes, values and positions.
positions is not use actualy but it could be usefull in the future.
- _indexes_ contains index of the collection,
- _values_ contains value of the collection,
- _positions_ contains the numerci position of the index value of the collection.
### Methodes or functions
- _getPosition_ return the free position of the collection.
- _addIndexValue_ with 2 parameters :
  - _index_ : the alias of your project.
  - _value_ : the path of your project.
  This methode set the collection with your list of aliases pathes for your projetcs.
- _getValueFromIndex_ with 1 parameter
  - _index_ : the alias of your project.
  Return the path of your project found from the index passed by parameter.
- _getlistOfCollection_, usefull to debug or just list your collection to see if indexes, values and positions contains the rights datas.
- _displayIndexes_ display the list of aliases configured. Used in goProject to list the alias possibilities if you dont set parameter after the command.
- _existIn_ function who return 0(true) or 1(false) if alias exist in the collection or not.

