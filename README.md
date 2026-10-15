# VIM-TERM

Run a command in Vim terminal and interact vim errors and locations in the output.

Inspired by vim-shout and Compilation mode of Emacs but use Vim's terminal emulator so you get real terminal features.

## Example usage

```vim9script
# I use `S` to change a line
nnoremap cc :silent! wa!<cr>:Term <Up>
```

Issue `cc` and type your compilation command.

Use `]]` and `[[` in the terminal buffer to move cursor to next and previous errors respectively.

Hit `<Enter>` when cursor is on an error to jump to its location in code in a split window.

Issue `cc` again. The command-line is filled with your previous compilation command so you can easily rerun it.

Repeat...
