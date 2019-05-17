# Vim 

## Motion

Command   | Description 
--------------------|--------------------
ctrl+e | Scroll screen up 10 lines 
ctrl+d | Scroll screen down 10 lines 


## Misc

Command   | Description 
--------------------|--------------------
:so $MYVIMRC | Reload vim config 
ga | reformat selected text


## Plugin Cheatsheet
*Assuming the leader key is `'`*

### EasyMotion

Command   | Description 
--------------------|--------------------
''b | Search backward any word
''w | Search forkward any word
''f {character} | Search forkward for character


### Surround

Objective   | Original | Command | Edited Text |
--------------------|--------------------|--------------------|--------------------|
Wrap line with symbol | Hello World! | ys$' | 'Hello World' |


### Syntastic

Command   | Description 
--------------------|--------------------
:SyntasticToggleMode |  Toggle Syntastic into passive mode, which will disable auto-checking.
:SyntasticCheck | Enable SyntasticCheck


Resources:
[Vim surround plugin tutorial](http://www.futurile.net/2016/03/19/vim-surround-plugin-tutorial/)
