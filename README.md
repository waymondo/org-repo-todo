This is a simple package for capturing and visiting todo items for the
repository you are currently within. Under the hood it uses `org-capture`
to provide a popup window for inputting `org-mode` checkboxed todo items
(http://orgmode.org/manual/Checkboxes.html) that get saved to a `TODO.org`
file in the root of the repository.

Install is as easy as dropping this file into your load path and setting
the relevent functions to keybindings of your choice, i.e.:

```
  (global-set-key (kbd "C-;") 'ort/capture-todo)
  (global-set-key (kbd "C-'") 'ort/goto-todos)
```
  
Using the `C-u` command prefix with either of these commands will
capture/visit the todos in your `user-emacs-directory' instead.
