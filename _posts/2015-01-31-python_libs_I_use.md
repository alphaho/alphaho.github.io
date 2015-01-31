---
layout: post
title: libraries I have been using in Python
---

After using python in our team for sometime to automate testing, I have find some libraries that are quite useful. Some of them are made to replace the standard libraries. Here are they:

|what for| library|
|:-------|----------:|
| Http Client | Requests |
| Data Analysis| Pandas|
|Path| path.py|
|server management | fabric|
|logging| logbook|
|time|arrow|
|file monitoring| watchdog|
|command line options| docopt|
|packaging|pyinstaller|
|dependency management|pip|

Among them, requests, pandas, path.py, docopt and arrow are the libraries that I heavily use.

#### requests
Until I get my hands on requests, I hates to deal with http requests in python, as I found the standard library in python for http client is very counter-intuitive. Now with requests, all you need is the function `requests.get(url)`. That's it. I would never need to deal with the different concepts again, for just making a http request!

#### arrow
Arrow is similar to requests. All you need is `arrow.get(time)`

#### pandas
Pandas is extremely good to do some data manipulation. In my company, people usually used the Excel for such task. But Excel is not that easy to integrate with other testing scripts and it's slow. What's worse, if the data set is too large, Excel will truncate the data! While using pandas, all the operations are very straight forward. Not only transforming, filtering, calculation, but also joining the two data sets as the way you want. And it won't mess up with your times as Excel would always do!

#### path.py
Path.py has put all the functions under one interface.

#### docopt
There was a time, I need to kicking my head thinking how can I give my scripts an elegant command line interface. As the standard library in python for the command line options is not very intuitive, and looks cumbersome. Now, docopt is the answer to my question! To write an elegant command line option, you just need to write the doc! This becomes one of my favourite libraries in python!
