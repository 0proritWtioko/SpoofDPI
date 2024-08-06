# Speedcrunch Download
  
Limit to suite:[buster][buster-updates][buster-backports][bullseye][bullseye-updates][bullseye-backports][bookworm][bookworm-updates][bookworm-backports][trixie][sid][experimental]Limit to a architecture: [alpha] [amd64] [arm] [arm64] [armel] [armhf] [avr32] [hppa] [hurd-i386] [i386] [ia64] [kfreebsd-amd64] [kfreebsd-i386] [m68k] [mips] [mips64el] [mipsel] [powerpc] [powerpcspe] [ppc64] [ppc64el] [riscv64] [s390] [s390x] [sh4] [sparc] [sparc64] [x32] You have searched for packages that names contain speedcrunch in all suites, all sections, and all architectures.Found **2** matching packages.
 
Search in specific suite:[focal][focal-updates][focal-backports][jammy][jammy-updates][jammy-backports][mantic][mantic-updates][mantic-backports][noble][noble-updates][noble-backports][oracular]Limit search to a specific architecture: [i386] [amd64] [powerpc] [arm64] [armhf] [ppc64el] [riscv64] [s390x] You have searched for packages that names contain speedcrunch in all suites, all sections, and all architectures.Found **1** matching packages.
 
**Download Zip ✵ [https://tinurll.com/2A0TbB](https://tinurll.com/2A0TbB)**


 
Thank so much for all the hard work you guys have put into this! I've been following this project for years. And for the longest time, I thought it was no longer being developed until I found the GitHub!
 
I use speedcrunch daily at work to make simple calculations.

But very often I use the feature from realease 0.10.1 to copy a calculation in input field by doubleclicking in the history.
I miss this feature in 0.11. So I downgrade again to 0.10.1.
 
I'm using SpeedCrunch on a daily basis as my programmer's calculator. It's great to see this project isn't dead and new important features get finally implemented.

A feature that I'm missing is to be able to select a different result format for each result line. At the moment the result format is set globally. However, it would be great if one could change the format of a result afterwards, e.g. by right clicking and choosing a different format from the context menu, keeping all the format of all the other results untouched.
 
I found this new version on google looking how to do modulo on speedcrunch (I still don't know how to do it) and updated to it.

It is ugly so I downgraded it. I think a theme to be more similar to 0.10 shouldn't be bad (I changed theme to default, but still it doesn't have good readability). Also, removing functionality for no reason doesn't look like a smart thing to do to me. Was really necesary to remove the keyboard? Maybe it would be better an option to disable it...

By the way, I'm sure you have put a lot of work and there are improvements under the hood, so don't take this the wrong way.
 
Congrats for the new release ! I'm sure lots of people were waiting for it (I know I was, especially for the Windows binary).

@Anonymous
For modulo, use the mod() function.
I agree that the new styles are a bit disconcerting, but I got used to the "Standard" style sooner than I thought. If you can't, maybe you should fill a feature request for a more cleaner style (or a way for the users to customize the styles from the GUI).

@Helder Correia: Thank you for your detailed explanation!

2): I forgot this feature of speedcrunch, but this feature cannot replace the old double click feature for me. 

3): The History dock window is more usable for me, but cannot replace the old double click feature for me too.

Why? 
I calculate at work everytime very similar dose calculations for cancer therapie radiation plans. So, for me it is more easy to find the correct former calculation, which I have to modifiy, if I see the result too.

1): This is complicate, because I am not the programmer of this great program.
Is it not possible to seperate between "single click and mark" and "double click"?
If not, I have no Idea.
 
@themroc: > Is it not possible to seperate between "single click and mark" and "double click"?

I'll think about something that will leave everyone happy (i.e. being able to select text and also allow fast expression recovery without having to copy and paste).

Your use case makes me wonder that defining a simple function is what you really need though. It sounds like what you do is just tweak parameters manually and see what happens to the result. If that's the case, I'm convinced you'll benefit from the soon to come feature that allows users to define their own functions.

Or maybe it would suffice for you if you could also see the results (say, on a tooltip) in the History dock?

It was definitely interesting to know about what you use SpeedCrunch for at work, thank you.

FYI, I've created a ticket that you can subscribe to follow this issue.
 
No keypad? Seems to be telling casual users wanted a good calculator to take a hike.

The new website is hilarious.

The aura surrounding the new release seems a bit too minimalistic.
 
@Nighted: Thanks for your feedback. I've addressed the keypad issue in the post and I have nothing to add at the moment. I'd love to hear why you find the website hilarious. Maybe you're using a browser that is not able to display it properly. If that's the issue, I'd need more info from you.
 
Thank you for the work!
Dead or not, I did not even realize it has not been in development since 2009. Have been installing on all computers for many years and cannot get through any of my university assignments, especially physics and calculus where the variables and history are invaluable, without it.

I do not remember using keypad ever so having it gone is a non-issue. Instead, having a side panel with history and variables tabs is much more useful.

Thank you for daily irreplaceable tool.
 
Thank you so much for SpeedCrunch! What follows is thankful criticism of the new 0.11 version:

1) The default font and the 3 color schemes are very hard to read. I hoped that there would be a "classic" color and font option to replicate the appearance of 0.10.1 but I couldn't find it.

2) There's no keypad option that I can find which I use sometimes and needs to be available for all my installs.

3) The placeholder for the results scrollbar is hard to see and quite small compared to 0.10.1.

4) I miss double clicking on a previous line in the history to pop it in the current calculation field. I understand that the previous lines can be highlighted and copied now but old habits are hard to change.

5) I would like very much to be able to enter: 1,300+600 to get 1900 - is this an option? In 0.10.1, commas are either the decimal place or they produce an error. It seems that 0.11 treats commas as a decimal point. Can there be an option to use a dot as the decimal point and just ignore commas? E.g. 4,396 is interpreted as 4396. I paste in numbers with commas as thousands separators a lot and this would really help.

Thanks again for working on Speedcrunch. I very quickly downgraded to 0.10.1 after trying 0.11. I look forward to future versions.
 
@Anonymous: Thanks for the feedback. Here's my replies to your remarks.

1) The font is now fully customizable via settings. You can even play with the size easily with Shift+Up/Down. Any color schemes are now possible and it's extremely hard to please everyone. However, you can also disable syntax highlighting.

2) I addressed the keypad issue in the article. I'd be very interested to know why you need it so much.

3) You can also scroll with the mouse wheel and PageUp/Down (with or without Shift).

4) Already addressed by someone else in the replies. Please follow =475 and ideally provide ideas.

5) This is the most debated detail in the history of SpeedCrunch. The issue is that it tries to please everyone with small compromises. Countries use comma and dot in a perfectly inverted meaning. What is a comma to you is a dot to someone else, and vice-versa. That's why the newly introduced digit grouping is done via a small gap instead. This is also why the function separator is a semicolon instead of a comma. That said, I think the app should be smart when it comes to pasted data and convert it automatically.
 
Hello,

first of all, thanks for developing such great software. I really don't know how long I use SpeedCrunch, and I'm very fine with the portable version (I never try the installer version).

1. I like dark themes, cause its easier to read later in the night. But why are you inconsequent at the docking windows? It would be more readable if the whole App follows the same theme/skin.

2. Maybe you're right with: "virtual keypad is against the SpeedCrunch philosophy", but why there couldn't be an option to show the keypad, if some users want to. As default it may be hidden, and still follow your philosophy.
I often use the keyboard, and rarely use the keypad, but sometimes I had use the keypad on remote machines that don't have the actual window focus, so its much faster (for short things).
Even for non-professional SpeedCrunch users the keypad has some recognition effect (MS Calc), from time to time some colleagues at office want to calculate something (on my PC), and they can use SpeedCrunch 0.10.x on my machine (cause they knew MS Calc), instead SpeedCrunch 0.11 I cannot put in front of them. So **\_I\_** need to start MS calc for them.

3. Why it isn't possible anymore to open more than one instance at the same time? I mostly have three or more instances of SpeedCrunch 0.10.x open (on different desktops at the same machine), and really often use two of them simultaneously. It would be great to see that "feature" back in 0.11.

4. SpeedCrunch seems to block keyboard-events that aren't for itself, i.e. the media keys on my keyboard doesn't function if SpeedCrunch window has focus. SpeedCrunch 0.10.x doesn't make problems at this point. My be it's possible to path these key events through.

Please don't take this critic personal, I like SpeedCrunch really, and honor your great work on it. I really like the dark theme and the better syntax highlighting, but for the moment I had to downgrade to 0.10.1.2.

Kind regards,
Mr.K
 a2f82b0cb4
 
