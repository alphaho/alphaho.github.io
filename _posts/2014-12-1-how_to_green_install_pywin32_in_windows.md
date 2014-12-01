---
layout: post
title: How to green install pywin32 in Windows
---


Sometimes we would not have the authorization to insatll pywin32 using the exe/msi package. So we need a way to green install pywin32 on our windows platform.

Just need to:

1. Copy the correspondent pywin32 folders/files into site-packages
2. Add `site-packages\pywin32-system32` into PATH variable \(as those DLL would be required to run it)

Then we are done.