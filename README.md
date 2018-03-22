``mpv-install.bat + umpvw`` <img src="https://rossy.github.io/mpv-install/mpv-document.png" align="right">
===================

This script sets up file associations for [mpv][1] on Windows, using [umpvw][4].

How to install
--------------

1. Make sure you have the latest build of mpv. Official builds are here:
   https://mpv.srsfckn.biz/
2. Download the zip: https://github.com/SilverEzhik/mpv-install/raw/master/mpv-install.zip
   <br>
   **Note:** Make sure you use the above link. Don't use GitHub's "Raw" links
   on the files themselves, since these have incorrect line-endings, which
   cause the script to crash. (See [#7][2].)
3. Copy the .bat files, umpvw.exe, and the .ico to the same directory as mpv.exe
4. Run ``mpv-install.bat`` as administrator. **Note:** For an unattended
   install, use the ``/u`` switch.
5. Use the _Default Programs_ and _AutoPlay_ control panels to make mpv the
   default player

What it does
------------

- Uses umpvw to use mpv in single instance mode, macOS style
- Creates file associations for several video and audio file types
- Registers mpv with the _Default Programs_ control panel
- Puts mpv in the "Open with" menu for all video and audio files
- Registers umpvw.exe so it can be used from the Run dialog and the Start Menu
- Adds mpv as an AutoPlay handler for Blu-rays and DVDs
- Works when reinstalled to a different folder than the one it was in
  previously. (File associations created by the "Open with" menu have trouble
  with this.)

What it doesn't do
------------------

- Add mpv to the ``%PATH%``
- Enable thumbnails for all media types (use [Icaros][3] for this)

How to uninstall
----------------

To remove all traces of this script from your computer, run
``mpv-uninstall.bat`` as administrator.

**Note:** This is not necessary if you want to reinstall mpv later (in a
different folder, for example,) only if you want to remove it completely. To
reinstall, just run ``mpv-install.bat`` again.

Disclaimer
----------

Should work on Windows Vista and up, tested with Windows Vista, 7, 8.1 and 10.
These scripts were written for personal use and released with the hope that
they would be useful, but without any warranty.

This is a quick tweak of the original install script, and may not work quite as well. Also, it does not (at least intentionally) modify the DVD/Blu-ray associations.

[1]: https://mpv.io/
[2]: https://github.com/rossy/mpv-install/issues/7
[3]: http://www.majorgeeks.com/files/details/icaros.html
[4]: https://github.com/SilverEzhik/umpvw
