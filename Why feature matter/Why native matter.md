> Good experience encourages. Bad experience demotivates. 

Native apps are written in Swift or Objective C, but more importantly, they use native components and follow system guidelines. 

Electron apps is a web browser with the only site you can open. They are written in JS, usually for all platforms (macOS, linux, windows, iOS, Android). Electron apps almost didn't use native components and didn't follow guidelines — each developer reinvents basic things. 

Let's check how it can affect you: 

# OS experience

Apps should provide native expirience. I created a short list of system-wide options, while I limited only by my expirience and you may expect other shortcuts-services:

-   System shortcuts: 
	-   '⌘ .' to cancel
	-   '⌘ ,' to open preferences and '⌘ w' to close
	-   '⌘ p' for printing 
	-   '⌘ g' to find next
	-   all other shortcust
-   use system services integration in right-click menu
	-   encrypt or sign text with PGP suite
	-   send a text to another app
	-   insert a photo from the iPhone camera
	-   Lookup a word 
	-   Translate the text (macOS Monterey) 
	-   Configure Substitutions, Transformations, Spelling, and Grammar 
	-   Search text
-   App option accessible via the menu bar
-   Automation support
-   Same UI expirience 
	-   Tabs
	-   Preferences
	-   Element placing and design language

Native macOS or iOS experience means you can learn system behavior once and use it for all apps: Mails, Calendars, Text Editors, Web Browsers, Task Managers, Notes, Photo Editors, Terminals, RSS readers, and any software which follows system guidelines. 

Native macOS and iOS experience mean you can open any app and use the knowledge you already have.

Native macOS and iOS experience mean you can use your intuition about app behavior and element placing. Intuition, which was created by other app usages. 

Because you need to learn only goal-specific primitives, Native experience makes the app learning curve lower → more fun. 


## Shortcuts

### Open preferences
The default shortcut for preferences in macOS is "⌘ ,". 

Native apps: all 
Electron apps: [[Notion]], [[Obsidian]] and [[HyperNotes]]

In [[Clover]], [[Logseq]], [[Mem]], [[Roam]] you will need to explore UI and find where you need to click: 
![[logseq-settings.mp4]]
![[roam-settings.mp4]]

### Close preferences
For closing preferences in macOS, press "⌘ w"

Native apps: all 
Electron apps: one of the apps

### Cancel operation
For cancel, press "⌘ ."
Native apps: all
Electron apps: one of the apps

## System integration on the right click

Native apps: all apps
Electron apps: none of the apps

## Menu bar
The menu bar is the heart of macOS. As a macOS user, I expect to do operations from the menu bar. It's a native and intuitive way for me (as a Mac user) to look up functions. 
  
Also, I'm user of 'Help→Search' scenario: 

![[help-hoteplan.jpg]]
![[help-bear.jpg]]

Native apps: has a rich number of items in the menu bar
Electron apps: only a few apps have few options like "preferences."

### Open preferences via the menu bar
Preferences are also accessible via the menu bar: press on the app name and choose preferences. 

![[menu-bar-native.jpg]]

Native apps: all apps
Electron apps: [[HyperNotes]]

[[Clover]], [[Logseq]], [[Mem]], [[Notion]], [[Obsidian]], [[Roam]] get you nothing. 


## Automation support
A lot of automation software (like Hook or Alfred) depends on the menu bar. 

I can define keyboard shortcuts to menubar items via 'System Settings' → 'Keyboard' → 'Shortcuts' → 'Application Shortcuts'
  
Apps like 'Paletro' depend on the menu bar. 

While Electron apps can provide some API for automation, most automation software will require you to learn this API before you can do anything. 

## UI experience
All native apps sharing the same or similar UI experience
Each Electron apps builds their own design language

### Preferences UI
All native apps share the same UI/UX for preferences — if they have multiple tabs — showing them with an icon at the top. As example: 
![[noteplan-menu-ui.jpg]]
![[craft-menu-ui.jpg]]

Each Electron app contains different UI/UX for preferences:

[[Clover]]
![[clover-menu-ui.jpg]]

[[HyperNotes]]
![[hyprenotes-menu-ui.jpg]]

[[Notion]]
![[notion-menu-ui.jpg]]

[[Obsidian]]
![[obsidian-menu-ui.jpg]]

### UI elements placing

Native experience — folders and notes on the left bar, notes on the right.

[[NotePlan]]
[[noteplan-ui.jpg]]

[[Bear]]
[[bear-ui.jpg]]

[[Craft]]
[[craft-ui.jpg]]

And same for [[iA Writer]], [[The Archive]], [[SimpleNote]]

In Electron apps, only [[Notion]] provides the same experience. 

[Obsidian]] and [[Clover]] uses the left bar for changing app mode, open commands, panels, and settings in addition to the note list.

[[obsidian-ui.jpg]]

[[Mem]] and [[Roam]] uses the left bar for mode changing

[[HyperNotes]] uses the left bar for changing view. The left bar disappears when you open a note.

[[Logseq]] didn't have a left bar and uses the right bar instead


# UI bugs
Based on my experience, Native apps contain less number of annoying UI bugs. Probably because they use system components instead of components provided by Electron for all systems:

Here is only few bugs I found while I created this text:
![[bug-ui-close-obsidian.jpg]]
![[bug-ui-obsidian.mp4]]
![[roam-bug.mp4]]
![[logseq-panel.mp4]]
![[obsidian-resize.mp4]]
![[mem-switch.mp4]]


Native apps have UI bugs as well. But usually, they are more minor and not that annoying.  

  

# Speed and resource usage

I tried to include 10,000 markdown files and check resource usage. 

[[NotePlan]] ~220mb
[[Craft]] (local files mode, 100,000 blocks) ~300mb
[[Obsidian]] ~900mb

Also, because Electron apps need to render all elements as HTML/CSS/JS — they consuming a lot of your graphic card resources.
It slows down your laptop/phone and uses more battery. 

Some Electron apps developers did a colossal job of making their application fast (like [[Obsidian]] - great job!). Still, usually, Electron apps are slower and have a measurable delay for navigating through notes and other elements. 


# Phone experience

Electron application feels even worse on your iOS — because of UI inconsistency and limited phone resources. 

Also, native developers tend to follow guidelines and best practices because they are using elements prepared by Apple. While Electron developers need to invent everything by themselves. 

The result is an experience like this ([[Obsidian]] mobile):

[[obsidian-mobile.mp4]]

  
# Conlusion

Native apps are intuitive, look better, feel better, faster, consume fewer resources, contain fewer UI bugs, are more automatable, share the same design language, and have similar UX experiences. 


Electron apps are not intuitive, slower, have more UI bugs, consuming more resources, require learning for basic things, are less automatable, use more system resources, and feel wrong. 

My recommendations: try to prefer native apps over Electron each time.