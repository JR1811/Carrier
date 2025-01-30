# Carrier
Easily move animals, chests and mob spawners!

### Port Information

This version makes use of he 1.19 version.
[ShiroJR1811](https://github.com/JR1811) ported it down to 1.18.2 to make use of the newest Fabric Loader version.
Code changes have been made to adjust Minecraft code changes due to porting down from 1.19 to 1.18.2.
Specifically Command registration events and text object creation were adjusted.
For more information check out the git commit content or read about it in the [Fabric Blog posts](https://fabricmc.net/blog/)

In addition, launching this mod on the server side (multiplayer), prevented the server from booting. A fix has been made
to some of the Carrier classes, such as `CarriableSpawner`, to at least have the fields listed on the server side, even
if they technically shouldn't be there. There should be a cleaner fix for that but the server instance seems
to boot just fine now. For more information check out which classes have been changed in the git commit.

ARRP version needed to be `0.6.4` since newer ARRP versions try to mixin into class fields
which don't exist yet in 1.18.2