# wide-ergonomic-keyboard-layouts
Type faster and more comfortably, just by changing your keyboard layout[(*)](#footnotes). 

![qwerty wide](images/qwerty%20wide.png)

# What is this about?

You have probably heard of alternative letter mappings like Colemak (or the nowadays obsolete Dvorak), and you also might have heard that a good ergonomic keyboard helps much more with typing comfort than any change in letter arrangement. So split keyboards are the best, cleave-type keyboards (like the class "Microsoft Ergonomic" line) are second best, and a wide keymap is what you use, if you don't have a fully split keyboard or don't have it with you when using your laptop. The basic idea is to have a more natural hand position, which helps to relax the shoulders (and a little bit your whole body). The side effect of doing this with a software mapping has some extra benefits:
 - it works on any keyboard, even laptops, and as an extra boost on cleave-type ergonomic keyboards;
 - it makes all the keys on the right side of the keyboard easier to reach (which matters a lot for Backspace and Shift!);
 - less keys are operated with the weak pinky finger and more with the strong index finger; 
 - and finally, brings your right hand a bit closer to your mouse.

So, in short, it gives you some benefits of an ergonomic keyboard without having to buy one; and it even improves the ergonomics of any ergonomic keyboard that is not fully symmetric. Here's a wide keymap on my old Microsoft Sculpt keyboard:
![MS Sculpt with wide German keymap](images/MS%20Sculpt%20with%20wide%20German%20keymap.jpg)

And here, one of two laptops that I switched to a wide keymap:
![Laptop with wide keymap](images/Laptop%20with%20wide%20keymap.jpg)

Both pictures show that even when the keyboard doesn't advertise swappable keycaps, you can swap keycaps. Just try it first with an unimportant key such as *Break* or *PrintScr* and you'll be on the safe side.

# What is there for Download?

Currently, there are only keymaps for Windows because I need someone to test any Mac version, even though it can easily be generated.

If you want to inspect the mappings or compile them yourself using MS Keyboard Layout Creator, check the `.klc` files in the repo. If you just want to get the keymap to install in Windows and use it, head to the [releases] tab.

# What about programmable keyboards?

Great Question! This repo doesn't have any wide-map config for any type of programmable keyboard because there's so much variation and also because it's so easy to configure these keyboards individually. If you want to try a wide keymap, just fire up your keyboard programming tool, move the letters (and other character keys) around, and within a few minutes you'll be able to try it. 

I made this repository mostly for use with laptops, for when you don't have an external keyboard around. Otherwise, I recommend that any external keyboard you buy should be programmable for several reasons:
 * you can use the wide-mod config on any operating system, even Android, iOS, ChromeOS which don't otherwise let you configure the keymap for physical keyboards.
 * you can add a nav-layer, so you don't need to reach far for the home/end and cursor keys if you just want to move a few characters/words back to fix a typo.
 * you can fix a lot of the awkward keyboard shortcuts like Windows Win+Shift+S for a screenshot; I just turned it into Fn+S.
 * and finally, you can also make other improvements to the base keymap, like swapping J and N or going full QWPR to minimize your finger movement during typing of long(ish) English messages or text (such as what I am just typing here, haha).

# I know Qwerty and Colemak, but what is Qwpr?

First of all, if you are used to the Qwerty or Colemak letter arrangement and want to try the wide key map, don't worry about Qwpr and go download and use the wide keymap for your layout.

If, however, you would like to try an improved letter mapping and want to avoid spending much learning time and the period of slow typing which comes with that, then Qwpr might be for you. 

![qwpr keymap](images/qwpr%20wide%20keymap.png)

As you can see on the picture, Qwpr only changes 10 letters (and semicolon) from their Qwerty position and all but P and E even stay on the same finger (if you are touch-typing). This makes it almost trivial to learn this letter mapping with some half-hours of practice at https://typ.ing. There's not much literature about this mapping, which was developed by Jameson Quinn, but my keymap comparator shows that it has [great metrics] for its easy learnability. That's why I included it here.

# Future Work -or- Why are there no other language-layouts here?

(*If you are looking for a wide keymap on the UK keyboard, there is one at [GitHub::stevep99/keyboard-tweaks/.../KLC](https://github.com/stevep99/keyboard-tweaks/tree/master/KLC).*) 

In short, two reasons:
 1. problems with the ISO keyboard layout.
 2. so many additional improvements are possible that I don't know where to start with, but you can easily make your own.

### What are those problems with the ISO layout?

 - first, the extra key next the left Shift becomes very annoying on a wide keymap. The wide keymap makes the right Shift much easier to reach, so that the left Shift suddenly feels much worse. Different people prefer different solutions to this:

   - a. make that additional key into a second Shift key, so that it behaves like the ANSI keyboard (with a big Shift key) only that the key is split in two.
   - b. use the Caps Lock key as a second Shift key. 

 - second, some characters need the AltGr key to be pressed, which (in touch-typing mode) is only reachable with the right hand. 
   That makes it very awkward to use together with keys on the right hand. This can be fixed by mapping a key on the left hand to be a second AltGr. Again, this could be either the old Caps Lock, or the extra ISO key.

When making those modifications, we have to map the original characters of that (now reused) extra ISO key somewhere on the AltGr layer, which is different for each language. And also, it's a trigger to optimize the AltGr layer for better usability, which leads us to the next point.

### What do you mean by "more optimizations"?

When I switched to a wide keymap, I took the right-hand keycaps off my keyboard to match them with the new keymap, and I just couldn't bring myself to put them back in their stupid Qwerty position: I immediately swapped J with N, and I with K, and then later also U with K. This simple swap is super-easy to get used to and makes typing a lot easier. (See the "cozy" and "qwpr" keymaps on my [comparison app] to see how it improves typing metrics.) But that's only one of many changes one can make! Another one is that on some keyboards, the J keycap cannot be put on any other key. This seems stupid at first, but can lead to a nice keymap with a ring swap of J, N, H.

The whole AltGr layer is another thing: in the German standard keymap many AltGr characters are mapped to the number row or some pinky keys while the home row has nothing mapped on the AltGr layer. So since we need to find a new place for the "ISO key characters" anyway, we can also make a few more optimizations. And since the AltGr layer is only sparsely used, we just leave the original mappings in place, so we won't be forced to always remember the new ones.

And it goes on like this: once you already downloaded the keymap editor for your system (like the MS Keyboard Layout Creator), it's easy to just make this or that additional change.


### Footnotes

(*) Actually, you change not the keyboard, but the "keymap", that is, what each key does when it is pressed. The "layout" is how the physical keys are arranged and you'd need a new keyboard to change it. See https://matey-jack.github.io/key-layout-visualizer/ for the difference.

[releases]: https://github.com/matey-jack/wide-ergonomic-keyboard-layouts/releases
[comparison app]: https://matey-jack.github.io/key-layout-visualizer/
[great metrics]: https://matey-jack.github.io/key-layout-visualizer/#layout=0&mapping=Qwpr&viz=4
