---
layout: post
title: Preserve the json order when reading into Python
---

By default, Python's json module won't preserve the order of the items in the json file. This makes sense as after reading in the data, it's a dict object in Python.

But there may be some cases that we would like to keep the order of each item in the json file we load into Python. We may read it as an OrderDict. And here's how:
	
	json.load(filename, object_pairs_hook=collections.OrderDict)
