[![MELPA](http://melpa.org/packages/org-repo-todo-badge.svg)](http://melpa.org/#/org-repo-todo)
[![MELPA Stable](http://stable.melpa.org/packages/org-repo-todo-badge.svg)](http://stable.melpa.org/#/org-repo-todo)

This is a simple package for capturing and visiting todo items for the
repository you are currently within. Under the hood it uses `org-capture`
to provide a popup window for inputting `org-mode` [checkbox list items](http://orgmode.org/manual/Checkboxes.html)
or regular `** TODO` items that get saved to a `TODO.org` file in the root of the repository.

#### Installation

Install from [MELPA](melpa.milkbox.net) with `package-install org-repo-todo`, or drop `org-repo-todo.el` into your load path.

#### Usage

Set the functions to keybindings of your choice, i.e.:

```
  (global-set-key (kbd "C-;") 'ort/capture-todo)
  (global-set-key (kbd "C-'") 'ort/capture-checkitem)
  (global-set-key (kbd "C-`") 'ort/goto-todos)
```

#### Config

###### `ort/prefix-arg-directory`
This is the alternate directory to capture to and visit when using the `C-u` prefix. The default value is `user-emacs-directory`.
