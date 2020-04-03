# VIM Help

### VIM general: 
	i -> INSERT-Mode befor cursor
	a -> INSERT-Mode after cursor
	:w -> write file
	:wq -> write and quit
	(SHIFT +) w -> going up a words
	(SHIFT +) b -> going back a word
	ctrl + n -> complete suggestion
	u -> undo last change
	U -> revert all change in the last modified line
	\ -> leaderkey (default)
	/ + <text> -> find <text>
	n -> search forward
	N -> search backward
	* -> search forward word on cursor
	G -> GoTo last line
	g + g -> GoTo first line
	q + {a-z} -> start recording
	q -> stop recording
	@ + @ -> run last recording
	@ + {a-z} -> run {a-z} recording
	V -> select line - then move to line - d -> cut / y = copy 
	P -> paste after
	CTRL + w + w -> switch between windows
	CTRL + w + <h,j,k,l> -> switch using movementkeys

## Addons
	
### NERDtree:
	:NERDtree -> open NERDtree
	I -> Toggle "show hidden files"
	t, T -> Open File in new Tab
	g + t -> next Tab 
	g + T -> previous Tab
	m -> Filesystem Menu
	i -> open selected file in horizontal split window
	s -> open selected file in vertical split windows
	R -> refresh the tree
	:Bookmark <name> -> move to folder to bookmark then type :Bookmark <name>
	B -> toggle Bookmarks
	D -> delete Bookmark

### EasyMotin:

### Syntastic:
	cs<SurroundingToReplace><SurroundingReplacedBy> -> replace surrounding with other surrounding		

### YouCompleteMe:
	CTRL + n/p, TAB, ENTER, SHIFT + S -> switch between sugesstions

### Tagbar:
	<F8> -> Toggle
	ds -> godef-split (horizontal)
	dv -> godef-split (vertical)
	dt -> godef-split (tab)

### Fugitive:
	:Gwrite -> Gwrite (not necessary)
	:Gcommit -> add commit message 
	:Gpush -> push to master ?!
