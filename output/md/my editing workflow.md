---
date: 2023-04-04
draft: true
sr-due: 2023-05-21
sr-ease: 271
sr-interval: 4
tags:
- inbox
- definition
- vim-tip
---

# My editing workflow

p* - pycharm only
n* - neovim only

I n daily life I use [pycharm](./pycharm.md) and [neovim (text editor)](./neovim%20%28text%20editor%29.md) inside
[kitty (terminal emulator)](./kitty%20%28terminal%20emulator%29.md).

Maybe in near future I will switch to use only neovim.


- [ ] files navigation

## Files navigation


- focus editor::`<c-'>`


- grep content in current project and open find toolbar::`<leader>fs`


- locate file in file manager::`<leader>pv`


- go to file::`<m-p>`


- [ ] recent files, Telescope oldfiles + cwd


- [ ] recent locations, [https://github.com/cbochs/portal.nvim](https://github.com/cbochs/portal.nvim)


- find file, with history and fuzzy search::`M-p`


- log git history of current file::`<leader>gl`


- get file local history::`<leader>u`

## Code navigation


- go to definition::`gd`


- go to declaration::`gD`


- find symbol, based on grep:`<leader>vws[S]`*


- find usages/references::`<leader>vrr`


- go to older/newer position::`<c-o>/<c-i>`


- hover help::`K`


- go to previous/current file::`c-^`


- go to previous/next function hunk::`[[`/`]]`

## Code editing


- code folding::`zo/zc/zr` *


- comment line::`gcc`


- comment block`gc<motion>`


- code formatting::`<leader>F`*


- code actions::`<leader>vaa`


- macro record/replay::`q<letter>/@<letter>`

## Code refactoring


- rename/move/extract/inline


- automatic refactorings (<!-- black integration -->)


- sort/organize imports

## Code autocompletion


- confirm autocomplete::`<c-y>`


- confirm copilot::`<tab>`


- snippets

## Code debugging/testing


- run debugger::`<f5>`


- restart debugger


- stop debugger


- step over


- step into


- step out


- run to cursor


- evaluate expression


- run/debug the nearest test::`<leader>pt`


- generate test


- run test


- coverage test

## Errors and warnings navigation


- go to next/previous error::`[d` `]d`


- go to file with error::?? traceback actions

## VCS


- add/remove into stage


- commit/push


- pull/rebase/merge


- diff


- push and create merge request
?
`git push -o merge_request.create --set-upstream origin HEAD`
key:


## harpoon n*


- [x] add file into harpoon list
      leader-a

- [x] show harpoon menu
      c-e

- [x] close harpoon menu
      q or esc

- [x] switch harpoon items
c-t c-n c-m-t c-m-n


- [x] from the quickmenu, open a file in: a vertical split with control+v, a horizontal split with control+x, a new tab with control+t

## Figutive


- [x] open diff/git for current file
  <kbd>=</kbd>


- [x] stage/unstage file
  <kbd>-</kbd>


- [x] commit chunk or selection of chunk
  <kbd>s</kbd>


- [x] commit staged changes
  cc


- [x] revert all changes, stash the changes
  czz Push stash. Pass a [count] of 1 to add
  `--include-untracked` or 2 to add `--all`.


- [x] czA Apply topmost stash, or stash@{count}.


- [x] dv Perform a |:Gvdiffsplit| on the file under the cursor.


- [x] dd Perform a |:Gdiffsplit| on the file under the cursor.


- [x] ds Perform a |:Ghdiffsplit| on the file under the cursor.


- [x] gt - accept left side of diff
- [x] gn - accept right side of diff


- [x] telescope git...
Telescope git_...

## Custom


- [x] quick switch to terminal
Ctrl-Z while editing in vim to send it to background, do your thing on the terminal and use fg at any time to bring up vim again.
C-\ switch to terminal


- [x] nvim term autoinsert mode


- [x] telescope builtin's, super search
  leader-f-F
  :h telescope.builtin


- [x] find commands, aka action search
  leader-f-a


- [x] search symbols [classes, variables, functions, etc.]
leader-v-w-s[S]


- [x] search files in current project
      <kbd>c</kbd>+<kbd>s</kbd>+<kbd>p</kbd>


- [x] search files in git repo
      <kbd>c</kbd>+<kbd>p</kbd>


- [x] pick file in current file directory (telescope-file-browser)
      <kbd>leader</kbd>+<kbd>p</kbd>+<kbd>V</kbd>


- [x] pick file in current project (telescope-file-browser)
      <kbd>leader</kbd>+<kbd>p</kbd>+<kbd>v</kbd>


- [x] find action, in vim case it's shortcut
      <kbd>leader</kbd>+<kbd>f</kbd>+<kbd>k</kbd>


- [x] open git commit UI, git status
      <kbd>leader</kbd>+<kbd>g</kbd>+<kbd>g</kbd>


- [x] git history
:G l or :G log


- [x] jump to source from git history
O or o


- [x] next/prev hunk
( )


- [x] stage hunk
s


- [x] unstage hunk
u


- [x] run debugger
      <kbd>f5</kbd>


- [x] restart debugger
      <kbd>leader</kbd>+<kbd>d</kbd>+<kbd>r[R]</kbd>


- [x] stop debugger
      <kbd>leader</kbd>+<kbd>d</kbd>+<kbd>x[X]</kbd>


- [x] diagnostics
      <kbd>leader</kbd>+<kbd>v</kbd>+<kbd>d</kbd>


- [x] declaration/definition ?? how it works
  leader-v-g-d[D]


- [x] rename
  leader-v-r-n


- [x] add/remove/list remove dynamic workspace folders
leader w a, leader w r, leader w l


- [x] vim-dadbod-ui [https://github.com/kristijanhusak/vim-dadbod-ui#mappings](https://github.com/kristijanhusak/vim-dadbod-ui#mappings)
full-featured database client, possible set values, load values from files, query, work with multiple databases


- [x] permanent bookmarks, marks, using viminfo?


- [x] linter, built-in into lsp


- [x] formatter
      leader-f


- [x] external documentation
      leader-zw search word
      gz <Plug>ZVOperator
      leader>z <Plug>ZVVisSelection
      <leader><leader>z <Plug>ZVKeyDocset


- [x] search in git repo (telescope-git)
- [x] list active buffers, to switch
c-a-p


- ~~Makefile integration~~
- [x] structure view
:TSPlaygroundToggle


- close splits
  c-w o


- equal splits
  c-w =


- maximize buffer
  c-w \_


- maximize buffer width
  c-w |


- switch to buffer
  c-w hjkl


- Undotree of file
  space-u


- Push changes
  leader-p
## Todo

- [x] telescope command_history


- [x] [https://github.com/harrisoncramer/nvim/blob/main/lua/plugins/neotest.lua](https://github.com/harrisoncramer/nvim/blob/main/lua/plugins/neotest.lua) check/use keybindings


- [x] refactoring
- pyton-rope arch package or rope
- pip install pynvim for neovim
- pip install ropevim
- install plugin
- on issues maybe need remov .ropeproject


- [-] JS debugging (browser)
Propably easly just use chrome built-in debugger/sourcemaps
[https://stackoverflow.com/questions/71810002/how-to-configure-the-dap-debugger-under-neovim-for-typescript](https://stackoverflow.com/questions/71810002/how-to-configure-the-dap-debugger-under-neovim-for-typescript)


- [-] ~~select in~~
- [x] new scratch file
:enew

- [x] execute current file
leader o or leader O (run using xdg-open)


- [x] add quotes/x pairs to words/sentence
[https://github.com/kylechui/nvim-surround](https://github.com/kylechui/nvim-surround)
[https://stackoverflow.com/questions/2147875/what-vim-commands-can-be-used-to-quote-unquote-words](https://stackoverflow.com/questions/2147875/what-vim-commands-can-be-used-to-quote-unquote-words)
```
    Old text                    Command         New text
--------------------------------------------------------------------------------
    surr*ound_words             ysiw)           (surround_words)
    *make strings               ys$"            "make strings"
    [delete ar*ound me!]        ds]             delete around me!
    remove <b>HTML t*ags</b>    dst             remove HTML tags
    'change quot*es'            cs'"            "change quotes"
    <b>or tag* types</b>        csth1<CR>       <h1>or tag types</h1>
    delete(functi*on calls)     dsf             function calls
```



- [-] vim shell output actions...
:h redir, !...|grep, r!... etc


- [x] run nearest test with debugger, show stderr output
Venv configured, filename is not `test.py`, but `test_*.py`

- [-] run group of tests with debugger, show stderr output
CI/Reporting

- [-] run debugger with specific configuration
run method?

- [-] ~~gitsigns.nvim~~ - overkill? vim fugitive is enough?
- [-] python lsp actions
    - [x] autoimport
    - [x] remove unused imports
- [x] python lsp symbols
- [x] optimize imports
- [x] copilot tab issue (try indent, while suggestion active!), markdown alignment issues
possible insert tab by S-Tab, but better to use S-Return


- [x] diff branches. Working tree diff.
- [x] compare working tree with branch
git-diff or :Merginal

- [ ] cherry-picking/compare
## Resources