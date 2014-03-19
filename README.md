# 6.005 Spring 14 Lecture 17: Thread Safety

Examples of confinement and using threadsafe collections.

Are the following thread-confined?

+ `SocialServer.friendsOf`
+ `RiskyStatic.cache`
+ `graph` in `SocialServer.makeFriendsGraph`
+ `socket` in `SocialServer.serve`
+ `Midi.midi`

Are the following strongly immutable?

+ `SocialServer.PORT`
+ `RiskyInstance`
+ `SocialServer.friendsOf`

Are the following safe for concurrency?

+ `graph` in `SocialServer.makeFriendsGraph`
+ the `Map` returned from `SocialServer.makeFriendsGraph`
+ `Midi`
+ `cache` in `RiskyStatic` or `RiskyInstance`
+ iteration over `friends` in `SocialServer.handle`
