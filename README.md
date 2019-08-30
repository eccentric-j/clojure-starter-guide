# Clojure Getting Started Guide

Welcome to Clojure. This guide will help you try Clojure for the first time using the ideal workflow to make sure you hit the ground running. Most getting started articles and guides are geared towards the one editor and workflow the author uses, which often means Emacs. This guide is written to help you get started with most contemporary editors so you can work with the editor you already know and love. If you run into any trouble please reach out in the Clojurians slack, Zulip, or create an issue.

## What is the ideal Clojure experience?

Aside from running and compiling Clojure code, there are two main components to get the most out of your Clojure experience:

1. Evaluate code immediately inline by connecting your editor to a Clojure REPL

It is a must-have for working with Clojure effectively. Connecting your editor directly to a REPL allows you to write a line or two of code, then send it to a Read-Eval-Print-Loop process that is running from inside your application. This ability allows you to change behavior, data, and functionality of your application immediately without having to restart your the process or wait for code to compile. Additionally, sending code directly to the REPL means it gets evaluated and the results immediately visible. Many editors will display the results in a pop-over just to the right of your code. This fast-feedback-loop lets you test drive any code before you even need to put it in a file giving you the benefits of test-driven-development without having to write tests in a separate phase of development.

2. Don't wrestle with parenthesis, let your editor do that for you

When coming to a LISP (**lis**t **p**rocessing) style language from a C-style language you may think to yourself, "What's with all the parenthesis?" Sure, it may feel jarring at first but once you let a structural-editing tool such as par-edit or parinfer do the thinking you'll soon find yourself dreading going back to managing everything yourself. Structural-editing can help in two major ways: The first is that they will often automatically balance parenthesis for you. The second either changes navigation to work with S-expressions `(<action> <param> <param> ...)` in systematic ways. For instance, you may see a binding called "slurp" that allows you to go from `(+ 1 2) 3` -> `(+ 1 2 3)` by pressing <kbd>shift+></kbd>.

This guide will help you connect your editor of choice to a REPL and get started with structural editing. However, not all editors have equal Clojure support so some may have further recommendations. We hope you will make sure you have both these core tenants running to provide yourself the most enjoyable Clojure experience possible.

## Setup your editor

We recommend you work with the editor you are most comfortable and familiar with. It's important to reduce the number of learning curves you are experiencing all at once.

1. VS Code
2. Atom
3. Spacemacs
4. Emacs
5. Vim
6. Cursive
