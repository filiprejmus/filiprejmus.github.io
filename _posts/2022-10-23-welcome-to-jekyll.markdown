---
layout: post
title:  "GSOC 2022 Report - React Native SDK for Jitsi-Meet"
date:   2022-10-23 12:09:21 +0200
---
Over the last four months I had the chance to contribute to [Jitsi Meet][jitsi-gh]. A popular feature of Jitsi is their offering of SDKs for React, iOS and Android which enables developers to embed a video conferencing feature in their apps including the complete capability of the Jitsi Meet app. As React-Native has become a big part of the mobile app development community and they missed a way to include Jitsi in their React-Native apps, the project idea got published on the GSOC ideas board.

### Project scope
After clarifying what the SDK needed to have with the community I proposed a React Native SDK that would expose React Native components with a similar functionality of the already known Jitsi Meet Native SDK classes. Interestingly enough, these Native SDKs are already utilising a React Native Component at their core that exposes Jitsi’s functionality for native mobile apps. Consequently, it was not necessary to rewrite all functionalities in React from scratch. After getting a great walkthrough from my mentors [Saúl][saghul] and [Titus][titus] we decided to create a SDK Component that would expose those exisiting components.
### Contributions
#### Pull Requests
##### Merged
  - [fix(prejoin) rename Prejoin.js to Prejoin.web.js](https://github.com/jitsi/jitsi-meet/commit/63ea273b201341e21fcb9a2167e34928d2615cc1)
  - [fix(ios) use the RN logger in RN modules](https://github.com/jitsi/jitsi-meet/commit/91cbeb0b3fd2ea67455050976ca4978681f4895a) 
  - [fix(helpers) move copyText function to web.js file](https://github.com/jitsi/jitsi-meet/commit/c3ebde18df3d8a6aa0f4dfad45ec4eb4dbbc648d)

##### Open
  - [ref(remove ReactInstanceHolder from AudioModule)](https://github.com/jitsi/jitsi-meet/pull/12439)
  - [feat(rnsdk) Create initial directory for React Native SDK (Main PR for the project)](https://github.com/jitsi/jitsi-meet/pull/11959)
  
#### Example repository
[Jitsi Meet SDK Example](https://github.com/filiprejmus/JitsiMeetSDKTester)

#### Open Tasks
- [ToDos that were too tricky to solve in time](https://github.com/filiprejmus/jitsi-meet/tree/create-react-native-sdk-directory/react-native-sdk)
- Add documentation to [Jitsi Handbook](https://jitsi.github.io/handbook/docs/intro/)
- React Native SDK tests for CI Pipeline

The open tasks that don't require a bigger reformating effort on Android side will be handled by me after the end of the GSOC project.

### Learnings and Conclusion
I remember the overwhelming feeling of being confronted with this huge codebase for the first time. Even with a clear project scope at hand it is hard to find an entry point. While nobody can or should skip the work of going through the code layer for layer, having a direct channel to Saúl and Titus anytime of the day was invaluable to the project's success. So if you are reading this because you want to apply for a future GSOC project, don't be afraid to reach out to the community forum or the Github issues page to get a better understanding! 
Working on this project really helped me become a better programmer. But what's more important: It helped me understand the immense value that open source has and that being a open source contributor is fun!
That being said thank you Saúl and Titus for teaching me so much!


[jitsi-gh]: https://github.com/jitsi/jitsi-meet
[saghul]:   https://github.com/saghul
[titus]: https://github.com/tmoldovan8x8
