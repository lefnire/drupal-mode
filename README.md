# Setup

Requires Emacs 24, which comes with package.el (see github.com/technomancy/emacs-starter-kit for more info, and github.com/nyuhuhuu/drupal-mode for previous versions).

Add Marmalade as a package archive source in ~/.emacs.d/init.el:

```Lisp
(require 'package)
(add-to-list 'package-archives
             '("marmalade" . "http://marmalade-repo.org/packages/") t)
(package-initialize)
````

Then you can install it:

    M-x package-refresh-contents
    M-x package-install RET drupal-mode RET