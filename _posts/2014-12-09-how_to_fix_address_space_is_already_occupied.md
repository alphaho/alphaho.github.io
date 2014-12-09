---
layout: post
title: How to fix Cygwin's "address space is already occupied" issue
---

After upgrading cygwin, we may sometimes run into the problem "address space is already occupied".

To solve this:

1. close all cygwin services
2. run `dash` as admin in the cygwin installation directory from Windows Explorer
3. in dash, run `/usr/bin/rebaseall -v`