# Emacs Interface to Common Lisp HyperSpec (CLHS)

## Usage

Add the following code to your Emacs init file:

```lisp
(autoload 'common-lisp-hyperspec "clhs" "Get doc on ANSI CL" t)
(define-key help-map "\C-l" 'common-lisp-hyperspec)
(custom-set-variables
 '(tags-apropos-additional-actions
   '(("Common Lisp" common-lisp-hyperspec common-lisp-hyperspec-symbols))))
```

## Description

Browse the Common Lisp HyperSpec documentation for the symbol at point.
Finds the HyperSpec at `common-lisp-hyperspec-root`.
With prefix arg, save the URL in the `kill-ring` instead.
