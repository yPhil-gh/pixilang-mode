# pixilang-mode

Emacs minor mode for editing Pixilang code

## Installation

Clone it directly in your load-path :

```sh
# cd ~/.emacs.d/elisp/
# git clone https://github.com/xaccrocheur/pixilang-mode.git
```

Make sure your load-path is recursive:

```lisp
(let ((default-directory "~/.emacs.d/elisp/"))
  (normal-top-level-add-subdirs-to-load-path))
```

And require it in your .emacs:

```lisp
(require 'pixilang-mode nil 'noerror)
```

See [[https://github.com/xaccrocheur/kituu][my dotfiles]] for an automatic implementation (that is, it is automatically installed on all my machines)

## Usage

```lisp
M-x pixilang-mode
```

To automatically load pixilang-mode when you visit a .pixi file, put this in your .emacs:

```lisp
(add-to-list 'auto-mode-alist '("\\.pixi\\'" . pixilang-mode))
```
