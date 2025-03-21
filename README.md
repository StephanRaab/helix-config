# helix-config

## Minor modes

`<v>` - select mode

`<g>` - goto mode

`<m>` - match mode

`<:>` - command mode

`<z>` - view mode

`<Z>` - sticky view mode

`<C-w>` - window mode

`<SPACE>` - space mode

## Key bindings to remember

`<C-u>` - page up

`<C-d>` - page down

`<A-.>` - repeat last motion

`<gn>` - go to next buffer

`<gp>` - go to previous buffer

`<%>` - select the entire page

`:sh` to run a simple shell command. I used this to run `:sh dotnet run` without quitting and then going back in every single time

`<i>`- insert before selection

`<I>` - insert at the start of the line

`<a>` - insert after selection

`<A>` - insert at the end of the line

`<e>` - go to end of word

`<r>` - replace current selection

`<E>` - go to end of word, and include chars

`<;>` - to remove current active highlighting

`<g>` - opens up a ton of movement options

`<g>` motion  + `<l>` - goes to the end of the line

`<gh>` -  goes to the beginning of the line

`<SPACE>` + `<?>` - opens up the command palette

`<space>` + `<f>` - fuzzy finder file picker

 -  `<C-n>` - scroll down

 -  `<C-p>` - scroll up

 -  `<C-v>` - open the file up in a vertical split

 -  `<C-wq>` -  close split buffer

`<C-c>` - comment out a line

`<mi>` + `[char]` - select everything within char

`<c>` - remove and go into edit mode

`<mr>` + `[char]` - select char and replace

 - `<mr">` and then `'` → this would select the double quotes and replace them with single quote

`<ms>` + `[char]` - surround selection in char

`</>` - to search
 - `<n>` to go to next instance of searched keyword

`<SPACE-/>` - to run a global search. 
- `<*>` do this before searching to copy selected word into buffer and have it ready when you do the global search

`<x>` - highlight current line. You can hit it again to grow selection down.

`<SPACE + r>` - rename a symbol

`<gd>` → go to definition

`<gr>` → show references with picker

If you start going down breadcrumb:

- <C-o> to go up a level

- <C-i> to go down a level

`<space + g>` - show you all files that you’ve changed in git

`<gw>` - go to 2 char label, aka mind control

`<]-f>` - go to next function

`<alt + o>` - grow selection

`<alt + i>` - shrink selection

`<">` - Access register menu

`<”+>` - access system clipboard → `<p>` to then paste 

`<shift + c>` - grow multi-cursor

- `<,>` to remove extra cursors 

## Find and replace

1. `<%>` to select the entire document
2. `<s>` to go into search mode
3. type in your selection, adding `\b` at the end for the regex pattern if it's supposed to be a direct match
4. hit `<enter>` to search
5. `<c>` to change with multiple cursors

## Remove all comments (example)
1. Select `\\`
2. `*` to add it to current register
3. `v` to go into select mode
4. `n` to select next
5. `gl` to select until the end of the line
6. `d` x2 to remove comment and remove blank space
