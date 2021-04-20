# Emacs Interface to Common Lisp HyperSpec (CLHS)

## Usage

Add the following code to your Emacs init file:

```lisp
(autoload 'clhs-doc "clhs" "Get doc on ANSI CL" t)
(define-key help-map "\C-l" 'clhs-doc)
(custom-set-variables
 '(tags-apropos-additional-actions '(("Common Lisp" clhs-doc clhs-symbols))))
```

## Description

Browse the Common Lisp HyperSpec documentation for the symbol at point.

Find the HyperSpec at `clhs-root`.

With prefix arg, save the URL in the `kill-ring` instead.
