---
layout: post
title: what I have used AHK's Hot String for?
---

When I started to used AHK, I found there's Hot String function is redundant to me. As it gives an example as:
```
::btw::by the way
```

I am not sure who would ever need such abbreviation for such a common phrase. While we want to use 'BTW', we just use it.

But after working for quite some time with different server accounts/passwords, file paths and urls, the need to fill in this annoying things come to me.

However, I have found that it seems every one around me keep using a cheatsheet txt file.
Every time one would need to use a server's login, he would 1. go to his file, 2. copy the username, 3. paste it to the login window, 4. then go back to the file again, 5. copy the password, 6. and paste it to the login window.
In total 6 steps! Just to login a server!(Yes, we are using windows remote desktop in our company...)

IT IS CUMBERSOME!

How can we simplify this? It would be good that if one can remember all of the username and passwords. But it seems there are too many to remember. Especially when some of them are seldom used.

Then there's a moment it comes to me that why not use Auto Hotkey's hot string?
Since then, my life starts to get easier.

I made my rules that:

1. to abbreviate the logins, postfix the env name with 'a' as the Account, and postfix the env name with 'p' as the password.

	For example, if one of the environment called SIT, we can name the account as `sita` and the password as `sitp`. So every time I need the account/password, I just need to put `sita`/`sitp`.
2. for the Paths that I often used, name it with the folder name postfixed with 'p'.

	For example, `/a/very/long/path/to/foledr/foo` can be abbreviated to `foop`.
3. for the urls that are usually used, use the first part, or combine the initial letter with its id.

	For example, we have urls like `foo.bar.baz`, it can be abbreviated into `foo`.

	Or urls are in the form of a common pattern with a unique id, like `foo123.com`, `bar123.com`, `baz456.com`, they can be abbreviated to `f123`, `b123`, `b456`.
	
	There's sometimes we would use the url with the protocol and port number, etc. We can abbreviate, for example, `https://foo123.com:1000` to be `hf123`.
	
Abbreviating the paths and urls not only makes it easy to type them to the prompt windows or address bar, but also makes your communication clearer in mails and in IM. As every time, it just take a few keystroke to get such a big chunk. The reader can know exactly what the paths/urls are.



Besides abbreviating the logins/paths/urls, another thing that I find I need to look it up every day is the standup conference call number.

As I use the cisco soft phone to dial in, I have save the conference number into a hot string under the phone context. Which means, such hot string will only effect when I am using the phone.

Thanks Auto Hotkey for making my life easier at work!