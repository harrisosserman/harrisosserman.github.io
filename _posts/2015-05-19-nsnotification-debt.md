---
layout: post
title: NSNotification Debt
---
**Disclaimer: NSNotifications are not iOS push notifications**

NSNotifications are signals that can be passed globally between classes in an iOS project.  Classes can send (or post) notifications to classes that listen for the notification.  For more information, check out the documentation <a href='https://developer.apple.com/library/ios/documentation/Cocoa/Reference/Foundation/Classes/NSNotification_Class/index.html'>here</a>
![image](https://images.bloggi.co/7b43cea9.png)

*Extensive use of notifications are bad for a number of reasons:*

**Notifications lead to poor software architecture** 
When building an iOS app, it’s very tempting to use NSNotifications to pass around signals.  Just because it is easy doesn’t mean that you should use them often.  Notifications are easy to use because the sender does not need to hold a reference to the receiver.  Therefore, your app could be poorly designed (from a software architecture point of view), but held together by crisscrossing notifications.

**Each notification can become gradually larger scoped than was initially desired**
It’s critical that each notification’s usage is defined.  Otherwise, it is very easy for a notification to become used for more than it was designed for.  For example, let’s say there is a ‘userChanged’ notification that would get fired every time that the user’s information was changed.  A name like this is often too vague because a lot of different things can change for a user.  Therefore, you will probably end up reloading/recalculating more parts of your app than are necessary, hurting the app’s performance.  A better name would be something like ‘userChangedContactInfo.'

**It’s hard to debug an app with lots of notifications**
When a notification is fired, more than 1 method can (and often is) executed.  Multiple code paths need to be investigated, which is annoying and time-consuming.