youdao-dict
===========

Youdao online dictionary query for Emacs in Linux

## Requirement

* GNU/Emacs or other Emacs
* Linux/OS X
* Curl
* Online
* [clippy.el](https://github.com/Fuco1/clippy.el)

## Installation

Make sure you are in Linux or OS X and have [curl](https://github.com/bagder/curl) installed.

Download or clone the repository and drop the directory into your `.emacs.d/`.

Load the files and requre the function like:

```lisp
(add-to-list 'load-path "~/.emacs.d/plugins/youdao-dict")
(autoload 'youdao-dict "youdao-dict")
```

## Usage

You can query a word by `M-x youdao-dict` or view detail by`M-x youdao-dict-detail. And you should add a keybinding:

```lisp
(global-set-key (kbd "key-you-like") 'youdao-dict)
(global-set-key (kbd "key-you-like") 'youdao-dict-detail)
```

`youdao-dict` show result using clippy
`youdao-dict-detail` show result using temp-buffer

## TODO

* Local storage
* Words table

## Author

[Yuanhang Zheng](http://www.zhengyuanhang.com)

## Thanks

* [popup.el](https://github.com/auto-complete/popup-el)
