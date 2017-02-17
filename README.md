# pac

pacur wrapper to mimic yaourts search feature

pac takes your arguments and just gives them to pacaur. Additionally it adds a few useful arguments and if none are
given except a search pattern it mimics the search function of yaourt and gives you a list of results. Then you just
type the package numbers you want to install instead of having to type the names.


Example of how the search function works:

```
$ pac chrome browser
1 extra/chromium 56.0.2924.87-1 [installed]
    The open-source project behind Google Chrome, an attempt at creating a safer, faster, and more stable browser
2 aur/google-chrome 56.0.2924.87-1 [installed] (1474, 39.50)
    An attempt at creating a safer, faster, and more stable browser (Stable Channel)
3 aur/chromium-gtk3 55.0.2883.87-1 (17, 2.77)
    The open-source project behind Google Chrome, an attempt at creating a safer, faster, and more stable browser (GTK3 version)
4 aur/google-chrome-dev 58.0.3013.3-1 (604, 1.67)
    An attempt at creating a safer, faster, and more stable browser (Dev Channel)
5 aur/google-chrome-beta 57.0.2987.54-1 (330, 0.98)
    An attempt at creating a safer, faster, and more stable browser (Beta Channel)
6 aur/ice-ssb 5.2.3-1 (12, 0.38)
    a simple Site Specific Browser for Firefox, Chromium and Google Chrome from "Peppermint OS" Project
7 aur/chromium-wayland 48.0.2548.0-2 (8, 0.00)
    The open-source project behind Google Chrome, an attempt at creating a safer, faster, and more stable browser
8 aur/browserpass 1.0.2-1 (0, 0.00)
    Chrome & Firefox browser extension for pass, a UNIX password manager
9 aur/browserpass-git 1.0.1.r8.5e8dced-1 (0, 0.00)
    Chrome & Firefox browser extension for pass, a UNIX password manager
10 aur/chromium-chromevox latest-1 (0, 0.00)
    Causes the Chromium web browser to automatically install and update the ChromeVox screen reader extention. Note: This package does not contain the extension code.
11 aur/tchrome 1.4-2 (0, 0.00)
    Close Chrome browser including background, or launch a version of Google Chrome/Chromium
==> Enter n° of packages to be installed (ex: 1 2 3 or 1-3)
==> -------------------------------------------------------
==>
```

Additional arguments:


| Argument            | Description                                                                      |
|---------------------|----------------------------------------------------------------------------------|
| `-a | --autoremove` | Removes orphan packages by issuing `pacman -Qdt` and removing the list it gets. |

