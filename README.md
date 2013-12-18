highlight-global
================

A highlight package for EMACS across all buffers/files.

Toggle highlight of current region(or symbol under cursor if region is not active)
``` lisp
(global-set-key (kbd "M-\"") 'highlight-frame-toggle)
```

Clear all highlight
``` lisp
(global-set-key (kbd "M-+") 'clear-highlight-frame)
```
