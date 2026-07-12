# kodi-fileposterview

This is for Estuary. It isn't perfect, but it will generate something similar to a poster with the file name for items that aren't in the library. 

![Screenshot](screenshot.jpg)

# Required changes

## 1. Copy

Copy `View_560_PosterFiles.xml` into the skin's `xml` directory.

## 2. Font.xml

Add to the **Default** fontset:

```xml
<font>
  <name>font8_poster</name>
  <filename>Roboto-Thin.ttf</filename>
  <size>16</size>
  <style>bold</style>
  <linespacing>0.85</linespacing>
</font>
```

## 3. strings.po

Add:

```po
#. viewtype name
msgctxt "#31990"
msgid "Poster Files"
msgstr "Poster Files"
```

## 4. MyVideoNav.xml

Add `560` to:

```xml
<views>50,51,52,53,54,55,500,501,502,560</views>
```

and include the new view:

```xml
<include>View_560_PosterFiles</include>
```

# Wishlist

- remove text box from `back`
- add cool overlay to make the captured thumbnails better looking
