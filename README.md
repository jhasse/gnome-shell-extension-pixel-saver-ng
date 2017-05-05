# Pixel Saver NG

This is a fork of [Pixel Saver](https://github.com/deadalnix/pixel-saver), with the difference that
it only works on GNOME 3.24 or newer because it removes a workaround for a
[bug](https://bugzilla.gnome.org/show_bug.cgi?id=781862) in earlier GNOME versions.

Pixel Saver is an extension for Gnome Shell that merge the activity bar and the
title bar of maximized window. It is especially interesting for small screens,
but MOAR pixels for your apps is always good!

The extension has no configuration. Its behavior is made to mimic the one of
the title bar and settings affecting the title bar should reflect in
Pixel Saver. It **Just Works**!

For applications using the modern GTK header bar, there are no space savings,
but the application title is still displayed in the top panel to achieve a
uniform appearance.

<table>
	<tr>
		<td><img src="title.png?raw=true" /></td>
		<td><img src="icons.png?raw=true" /></td>
	</tr>
	<tr>
		<td colspan="2">The title bar is completely gone and integrated to the activity bar.</td>
	</tr>
</table>

It is largely inspired by [bios and mathematicalcoffee's Window Buttons Extension](https://github.com/mathematicalcoffee/Gnome-Shell-Window-Buttons-Extension) and [mathematicalcoffee's maximus extension](https://bitbucket.org/mathematicalcoffee/maximus-gnome-shell-extension) and some code come from there. You may want to check theses out, especially if you want something more configurable.

Installation
------------

Install it with one click from the [GNOME extension repository](https://extensions.gnome.org/extension/723/pixel-saver/).

You can also follow these simply instruction for manual installation :

    git clone https://github.com/jhasse/gnome-shell-extensions-pixel-saver-ng
    cd gnome-shell-extensions-pixel-saver-ng
    ln -s $PWD/pixel-saver@deadalnix.me ~/.local/share/gnome-shell/extensions/pixel-saver-ng@bixense.com
    gnome-shell-extension-tool -e pixel-saver-ng@bixense.com

For code changes to become effective, you might need to reload GNOME Shell
by pressing <kbd>Alt</kbd> + <kbd>F2</kbd> and entering <kbd>r</kbd> .

### Dependencies

Pixel Saver depends on Xorg's xprop and xwininfo utilities. If not already
present on your system, these can be installed using:

* Debian/Ubuntu: `apt install x11-utils`
* Fedora/RHEL: `dnf install xorg-x11-utils`
* Arch: `pacman -S xorg-xprop`

Screenshots
-----------

If you want to see what the full desktop look like with this extension, you can check out what an
[unmaximized window](unmax.png?raw=true) looks like, as well as a [maximized one](max.png?raw=true).
