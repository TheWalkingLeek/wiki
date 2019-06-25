**{leader} is set to ,**

## Default
* i = insert
* v = mark
* y = copy
* x = cut
* p = paste
* shift + v = mark lines
* u = undo
* :nr = jumpTo nr
* :w = write
* :q = quit
* ?wort = search for wort
* ctrl + r = redo
* ctrl + p = explorer
* dd  = delete line
* ciw = delete word and enter insert mode
* ctrl+w -> v = vertical split
* ctrl+w -> s = horizontal split
* in visual -> shift+0 = formats selected
* ctrl+n = auto-complete
* :%s/find/replacewith/gc: find & replace
* ctrl+o: jump to prev. file
* :E -> %: adds new file in current directory
* ctrl+z -> fg: ctrl+z sets vim into background so you can use the shell and fg goes back

## vim-surround
* cs{toReplace i.e "}{with i.e '}: replaces the surrounding {toReplace} with {with}
* ysiw: adds surrounding smth to iw
* V -> S: Adds surrounding html tags to selected area


## vim-rails
* gf = regards context and jumps to file
* :E{resource}: Jumps to {resource} of this kind. I.E currently in people_controller.rb, Emodel --> person.rb
* :T{resource}: Same as above but opens new tab
* :V{resource}: Same as above but creates vertical split
* :S{resource}: Same as above but creates horizontal split
* :Rails console: obvious, ain't it?
* :Generate {name}: Does the rails g command in vim

## vim-fugitive
* Gstatus: Opens git status
* Gblame: Shows git blame for every line. Use Enter on a line to show differences

## CtrlP
* ctrl+p: pretty obvious
* in ctrlp -> ctrl+b: tab back
* in ctrlp -> ctrl+f: tab forwards
* in ctrlp -> F5: refresh ctrl+p detected files

## Nerdcommenter
* {leader}cc: normal one line comment
* {leader}cm: multiline comment
* {leader}cs: sexy multiline comment
* {leader}cl: comment current line
* {leader}cu: uncomment lines

## Vim Explorer
* %: new file
* -: up the hierarchy
* R: rename
* {delete}: delete