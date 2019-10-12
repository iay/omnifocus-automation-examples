# `omnifocus-automation-examples`

This project contains examples showing ways to use the new automation features
in OmniFocus.

These are stripped-down versions of things I use myself, tweaked to remove
some of the references to my own database. I have set their labels to start
with "x" so that they will (probably) appear at the end of your Automation list.

* **Defocus:** This works just like the standard "Unfocus" menu item when
  you are focused on something. It differs from the standard Shift+Command+F
  keybind in that it does not change meaning if nothing is focused.

  As with "Focus: Home" below, this has no effect in iOS versions of OmniFocus
  at the time of writing.

* **Focus: Home** Focuses down on a particular set of projects or folders.
  As an example, I've just included a couple of top-level folders from my
  own database, so you'd have to edit this to make it useful elsewhere.
  For example, you might have top-level folders representing clients and want
  the ability to focus on a single client or on all of them (but excluding
  non-client items). You can focus on any mixture of folders and
  projects that you can navigate to through the API.

  Note that, at the time of writing, this only works on the macOS version of
  OmniFocus.
