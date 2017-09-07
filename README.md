# MarkMyWords

A minimal markdown editor

**Status**: work in progress

Installation:
* AUR package by [emersion](https://github.com/emersion) at https://github.com/emersion/aur-markmywords
* PPA: _ppa:voldyman/markmywords_
  
  ```shell
  sudo add-apt-repository ppa:voldyman/markmywords
  sudo apt-get update
  sudo apt-get install mark-my-words
  ```
* openSUSE package:

  ```shell
  sudo zypper ar -f obs://X11:Pantheon pantheon
  sudo zypper ref
  sudo zypper in markmywords
  ```

## Screenshot

![screenshot](https://github.com/voldyman/MarkMyWords/raw/master/screenshots/screenshot-2015-1-29.png)

Author: Akshay Shekher

## How to build

```shell
sudo apt-get install libwebkit2gtk-3.0-dev 
sudo apt-get install libgtksourceview-3.0-dev
sudo apt-get install valac
git clone https://github.com/voldyman/MarkMyWords.git
cd MarkMyWords
mkdir build && cd build 
cmake -DCMAKE_BUILD_TYPE=Debug -DCMAKE_INSTALL_PREFIX=/usr ../
make
```

## Todo

- [x] Markdown Parsing
- [x] Live Preview
- [x] File IO
- [x] State management
- [x] Monitor file for changes
- [x] Export HTML
- [x] Export PDF
- [x] Preferences
- [ ] Github markdown
- [ ] Versatile keybindings
