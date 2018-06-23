# Visualising Toxic Code
Docs and links for my talk at the Thoughtworks UK 2018 away day

This repo is mostly so I can provide a single landing page for
people who want to view my source code, or demos.  It's pretty thin
right now, I'll hopefully be adding bits at the last minute!

## This page is at https://goo.gl/pRixSF

```clojure
(def magic-talk-code 175980)
```

## Live demos used in the talk

[The toxic code explorer demo](https://kornysietsma.github.io/toxic-code-explorer-demo-twuk2018/index.html)

[The git CD chart demo](https://kornysietsma.github.io/git-cd-chart-twuk2018/index.html)

## Toxic Code Explorer

Source code for the demo is at https://github.com/kornysietsma/toxic-code-explorer-demo - see the README there for more background.

The demo used in the talk has some minor tweaks and more code samples - https://github.com/kornysietsma/toxic-code-explorer-demo-twuk2018  - this will probably get deleted after the away day.

## Tools used to parse code for the Toxic Code Explorer:

(from the [project readme](https://github.com/kornysietsma/toxic-code-explorer-demo) )

* [cloc2flare](https://github.com/kornysietsma/cloc2flare/) which takes the output of `cloc` and produces flare files
* [csvmerge2flare](https://github.com/kornysietsma/csvmerge2flare/) which takes the output of [code-maat](https://github.com/adamtornhill/code-maat) and merges it with the flare files
* [indent2flare](https://github.com/kornysietsma/indent2flare/) which merges indentation data into the flare files
* [pruneflare](https://github.com/kornysietsma/pruneflare/) which I use to prune out things like vendor source code from flare files.

# Git Continuous Delivery charts

Source code for the CD chart demo is at https://github.com/kornysietsma/toxic-code-explorer-demo-twuk2018

I plan to put up a cleaner version of this in the not-too-distant-future.

The git logs are built using a clojure application which uses the open-source jgit library under the covers.
I haven't cleaned this up enough to upload it yet!

In a real project, you'd probably want to customise this to match your own CD and artifact management practices anyway.

# More random resources

Want to see more of the joy of the Linux kernel's git usage? Have a read of this:  https://www.destroyallsoftware.com/blog/2017/the-biggest-and-weirdest-commits-in-linux-kernel-git-history
