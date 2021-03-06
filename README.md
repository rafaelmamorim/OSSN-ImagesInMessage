# OSSN-ImagesInMessage
An improvement on OssnMessages component to allow the user to attach images. Images also appear properly into OssnChat component, but isn't possible (yet) to send images through this component.

If [FancyBox component](https://www.opensource-socialnetwork.org/component/view/369/fancybox) is enabled, images can be open in fullscreen mode.

## Screenshots
Screenshot of OssnMessages component
![Screenshot of OssnMessages component](https://www.rafaelamorim.com.br/temp/ImagesInMessage.png)

Screenshot of OssnChat component
![Screenshot of OssnChat component](https://www.rafaelamorim.com.br/temp/ImagesInMessage1.png)

## Changes

- Version 2.1
    - Fixed issue #10, found by Michael Zülsdorff
- Version 2.0
    - Added desandro/imagesloaded JS file and other stuffs to fix #9
    - Added code to delete file when user delete message. Files from deleted messages will keep into server. Sorry :-P
    - Added code to delete file if user leave or reload page. Working in Chrome, Firefox, Edge.
    - Added button to delete an image before send. If user select another image, the old is deleted too.
    - JS file splited in two, to not inflate head section.
    - Before upload is complete, send button is disabled
    - Added TESTS.md, with test sequence used on this version
    - Images now are stored in OSSN_DATA/messages/photos/{user id} folder. Sorry for don't do this in previous versions ( Issue #1 )
    - When user is deleted, folder and files are removed too.
- Version 1.2.1
    - Add credits to Open Social Website Core Team and OpenTeknik LLC for code used
    - Improved friendly name of component. "Allow to send images in OssnMessages" doesn't sound good to me :-)
- Version 1.2
    - Fixed issue #5, found by Michael Zülsdorff 
    - Fixed issue #6, found by Michael Zülsdorff 
    - Add translation in Spanish. Thanks, (Hugo Cuellar)[https://github.com/Erassus]
- Version 1.1
    - Fix cache issue #2. Tested in both scenarios (cache on and off). 
    - Fixed issue #1, after suggestion of @lianglee. However images sent using version 1.0 of component wont appear anymore. It's necessarily an issue to fix?
    - Fixed issue #3 (Notification shows [image=ME95bis5L0pxaC9ncUozVGo1M... instead a friendly message)
- Version 1.0
    - First release, with few tests. Use in production by your own risk.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[OSSN v4.0](https://www.opensource-socialnetwork.org/licence/v4.0.html)