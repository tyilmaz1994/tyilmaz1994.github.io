---
layout: post
title:  "Telegram Rss Service"
subtitle: "Rss Tracker"
date:   2018-09-06 23:34:01
categories: [projects, documentation]
---

## [Deprecated] Theese instructions are renewed. You can find out communicating with `[Link Text](https://web.telegram.org/#/im?p=@RssServiceBot)` what is change...

Project is briefly gets updates from RSS using telegram bots via telegram groups or channels. 

## How to use ?

Firstly, communicate telegram bot named as `@RssService` in order to get updates. There is only one command.

Command: `/start`.

When the command is called, `@RssService` shows menu as follows
![start screen command](/assets/images/startScreen.jpg)

`1-Channels` button shows three options.

* **List Channels:** shows all channels. If any channel is chosen, `@RssService` list all  added RSS. in order to get updates to channel, choose one of the listed RSS.

* **Remove Channel:** removes added channels. `@RssService` shows `unbounded` channels. If you want to remove `bounded` channel, firstly remove RSS from channel *(Rss > List Rss > {Chosen Rss} > {Chosen Channel})*. *(bound: RSS is added to channel or group in order to get updates, unbound: Remove RSS from channel or group in order to `not` get updates)*

* **Add Channel:** add channel to list. When `Add Channel` option is chosen, `@RssService` produce code. Ex;{% highlight python%}zJV7FXPiRlhvBbn3sjdebGI0ugDVv8XFHYBvzgfzBqWuevsDDV{% endhighlight %}this code must be sent to channel that contains `@RssService` as administrator within any privilege.

`2-Groups` button shows three options.

* **List Groups:** shows all groups. If any group is chosen, `@RssService` list all added RSS. in order to get updates to group, choose one of the listed RSS.

* **Remove Group:** remove added groups. `@RssService` shows `unbounded` groups. If you want to remove `bounded` group, firstly remove RSS from group *(Rss > List Rss > {Chosen Rss} > {Chosen Group})*. *(bound: RSS is added to channel or group in order to get updates, unbound: Remove RSS from channel or group in order to `not` get updates)*

* **Add Group:** add group to list. When `@RssService` is invited to any group, the group will be added to list.

`3-Rss` button shows three options.

* **List Rss:** shows all RSS that is added by you. If any RSS is chosen, `@RssService` list all `bounded` groups and channels. After channels and groups are listed, choose one of the below in order to `unbound` RSS to channel or group.*(bound: RSS is added to channel or group in order to get updates, unbound:Remove RSS from channel or group in order to `not` get updates)*

* **Remove Rss:** removes added RSS. `@RssService` shows `unbounded` RSS. If you want to remove `bounded` RSS, firstly unbound rss from group or channel *(Rss > List Rss > {Chosen Rss} > {Chosen Channel or Group})*.

* **Add Rss:** adds rss to list. After options is chosen, send RSS URL to `@RssService` as message. Last step is, send alias name for URL. this alias name will be used in `@RssService` menu. `@RssService` will show you alias name instead of URL in `@RssService` menu.

## Features

* new command `/bugreport` is added. You can report any bug, issue or advise using this command.(2018-11-18)
* system is renewed. Everything is changed (2019-11-24)
