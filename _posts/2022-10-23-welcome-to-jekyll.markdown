---
layout: post
title:  "GSOC 2022 Report - React Native SDK for Jitsi-Meet"
date:   2022-10-23 12:09:21 +0200
---
Over the last four months I had the chance to contribute to [Jitsi Meet][jitsi-gh]. A popular feature of Jitsi is their offering of SDKs for React, iOS and Android which enables developers to embed a video conferencing feature in their apps including the complete capability of the Jitsi Meet app. As React-Native has become a big part of the mobile app development community and they missed a way to include Jitsi in their React-Native apps, the project idea got published on the GSOC ideas board.

## Project scope
After clarifying what the SDK needed to have with the community I proposed a React Native SDK that would expose React Native components with a similar functionality of the already known Jitsi Meet Native SDK classes. Interestingly enough, these Native SDKs are already utilising a React Native Component at their core that exposes Jitsi’s functionality for native mobile apps. Consequently, it was not necessary to rewrite all functionalities in React from scratch. After getting a great walkthrough from my mentors [Saul][saghul] and [Titus][titus] we decided to create a SDK Component that would expose those exisiting components.

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}


[jitsi-gh]: https://github.com/jitsi/jitsi-meet
[saghul]:   https://github.com/saghul
[titus]: https://github.com/tmoldovan8x8
