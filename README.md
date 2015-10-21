highlight-global
================

A highlight package for EMACS across all buffers.

Unlike [`highlight-symbol`](https://github.com/nschum/highlight-symbol.el) which only does highlighting in the current buffer, this package highlights all matches across ALL buffers. Multiple highlights are supported. Different highlights show in different faces.

There are 2 ways to select a highlight target:

1. Mark the selection by region (very usful when you want to highlight a pattern accross all symbols).
2. Put cursor on a symbol to pick the symbol to highlight.

Once you have chosen a highlight target, you can call `highlight-global-hl-frame-toggle` to highlight/unhighlight the target. You could bind a key like this:

``` lisp
(global-set-key (kbd "M-H") #'highlight-global-hl-frame-toggle)
```

You could have highlighted multiple targets with different faces, but you want to clear all the highlights since you do not need them anymore. You could select the highlighted target one by one, then call `highlight-global-hl-frame-toggle` on each of them. Or you could just call `highlight-global-clear-hl-frame` which will unhighlight all highlighted target. You could bind it to a key as follows:

``` lisp
(global-set-key (kbd "M-+") #'highlight-global-clear-hl-frame)
```
