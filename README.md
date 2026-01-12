# rM Hacks

This is a collection of minor quality-of-life improvements for the
[reMarkable](https://remarkable.com) paper tablets.

## Disclaimers

This repository contains patches and modifications for third-party software,
which are provided "as-is" and without warranty of any kind, express, implied,
or otherwise, including but not limited to the warranties of merchantability,
fitness for a particular purpose, and non-infringement.

The patches provided here are intended to enhance or modify the functionality of
the respective third-party software, and their use is at your own risk.

Please note that the original software is subject to its own licensing terms
and conditions, and this disclaimer only covers the patches and modifications
provided within this repository. Ensure that you comply with the original
software's licensing requirements when using these patches.

These patches have only been tested on the 
[reMarkable Paper Pro Move](https://remarkable.com/products/remarkable-paper/pro-move)
tablet and only on the OS versions explicitly listed in each qmd file.

## How to install?

1. ⚠️ Carefully read the Disclaimers section above
2. Read the instructions [here](https://github.com/asivery/rm-xovi-extensions)
including the Disclaimers section
3. If you still want to proceed, install `xovi` and the `qt-resource-rebuilder`
extension
4. Build hashtab by running `xovi/rebuild_hashtable` (you will need to repeat
this step after every software update)
5. See the table below to choose the extensions you want and download them into
`/home/root/xovi/exthome/qt-resource-rebuilder/` on your device
6. Restart xovi
7. Consider installing
[xovi-tripletap](https://github.com/rmitchellscott/xovi-tripletap)

## Extensions

| Name | Credit | Comment | Reasons not to install |
|------|--------|---------|------------------------|
| clearScreenBeforeLocking.qmd | myself | This one is to solve a very specific problem of ghosting on the suspend screen when a colorful picture is selected (whether via [random-suspend-screen](https://github.com/asivery/rm-xovi-extensions/tree/master/random-suspend-screen) or simply by replacing `/usr/share/remarkable/suspended.png`). If you have no idea what I'm talking about, you don't need it. | It introduces extra flickering during screen lock, which is very visible. |
| enableExtraPenOnMove.qmd | [ingatellent](https://github.com/ingatellent/xovi-qmd-extensions) | It's a shame that reMarkable decided to remove such a useful feature on [Paper Pro Move](https://remarkable.com/products/remarkable-paper/pro-move). | It eats up space in the toolbar. |
| eraseSelection.qmd | [FouzR](https://github.com/FouzR/xovi-extensions)¹ | Allows using selection tool to erase. Compared to the FouzR's version, erasing preserves current clipboard contents. | N/A |
| forceRefreshGesture.qmd | [asivery](https://github.com/asivery/rm-hacks-qmd) | Force refresh the screen by touching it with five fingers. It's a built-in (though disabled by default) feature of xochitl. It helps remove any accumulated ghosting. | N/A |
| gestures.qmd | myself | Simple gestures to switch between pens and the selection tool. | It creates extra learning curve for the users, and makes scrolling more difficult (you need to swipe strictly in the center). |
| hideCloseButton.qmd | [asivery](https://github.com/asivery/rm-hacks-qmd) | Removes the button that I never use. Doing so frees up some space in the toolbar (e.g. for the second pen). | It creates confusion for the first-time reMarkable users (until they learn that you can close a document with a swipe from the top). |
| instantFavorites.qmd | myself | Removes delayed automatic rearranging of the recents/favorites. Once you pull down the document drawer (swipe with two fingers from the top), whatever gets displayed there first stays, so you can tap on a document immediately without waiting for it to finish updating. | You _will_ sometimes see outdated information in the document drawer. |
| toolbarIcon.qmd | [FouzR](https://github.com/FouzR/xovi-extensions)¹ | Displays some info about the currently selected tool inside the hide/show toolbar button, but in a very non-invasive way. When black pen is selected, it is designed to not show any changes. | It is not as useful without gestures. |
| uncompressDock.qmd | [NohamR](https://github.com/NohamR/xovi-qmd-extensions) | Replace the + button in the document navigator with the actual icons. | It is not immediately clear what the buttons do, unless you have used them before. |

¹ with modifications


## References

Similar collections of rmHacks:
* https://github.com/asivery/rm-hacks-qmd
* https://github.com/rmitchellscott/xovi-qmd-extensions
* https://github.com/ingatellent/xovi-qmd-extensions
* https://github.com/NohamR/xovi-qmd-extensions
* https://github.com/FouzR/xovi-extensions
* https://github.com/StarNumber12046/xovi-qmd-extensions/tree/main
* https://github.com/hegzploit/xovi-toolbar-extensions
