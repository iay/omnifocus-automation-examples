# `omnifocus-automation-examples`

This project contains examples showing ways to use the new automation features
in [The Omni Group][]'s [OmniFocus][] personal task manager.

These are stripped-down versions of things I use myself, tweaked to remove
some of the references to my own database. I have set their labels to start
with "x" so that they will (probably) appear at the end of your Automation list.

## Focus Plugins

One of the great features in the Pro version of OmniFocus for the Mac is the
ability to temporarily restrict your universe to a specified set of folders
and projects. This can be a bit fiddly, so these plugins make it easy to bind
focus operations to a shortcut key.

Note that, at the time of writing, these have no effect on the iOS version of
OmniFocus, Pro or otherwise.

* **Defocus:** This works just like the standard "Unfocus" menu item when
  you are focused on something. It differs from the standard Shift+Command+F
  shortcut in that it does not change meaning if nothing is focused.

* **Focus: Home** Focuses down on a particular set of projects or folders.
  As an example, I've just included a couple of top-level folders from my
  own database, so you'd have to edit this to make it useful elsewhere.
  For example, you might have top-level folders representing clients and want
  the ability to focus on a single client or on all of them (but excluding
  non-client items). You can focus on any mixture of folders and
  projects that you can navigate to through the API.

## Funnel Selection: Promote/demote

One part of my current workflow involves selecting candidates from a large
number of available actions, and further selecting from that group a small
number to be given immediate attention. I manage this with some perspectives and
two tags: "▶️ Next" signifying the first level of selection and "☀️ Today"
(which I also use as my forecast tag) signifying the second.

The **Promote/demote** plugin helps me manage this: bound to a shortcut key, it
will adjust these tags on the selected task or tasks:

* A task with neither tag is promoted to the first level by being given
  "▶️ Next".
* A task with "▶️ Next" is promoted to the second level by having that tag
  replaced by "☀️ Today".
* A task with "☀️ Today" is demoted back to the first level by having that tag
  replaced by "▶️ Next".

This plugin _works_ on iOS, and is reasonably convenient to use on the iPad
because the automation menu icon appears in most of the contexts you'd want
to apply this plugin. On the iPhone, though, the automation menu icon isn't
present in a lot of situations: until that changes, it's probably easiest to
swipe right on individual tasks and use the "Tag" and "Flag" actions. This is
one reason why I use "☀️ Today" as my forecast tag.

[OmniFocus]: https://www.omnigroup.com/omnifocus
[The Omni Group]: https://www.omnigroup.com
