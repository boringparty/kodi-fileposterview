# kodi-fileposterview
Makes a poster view for files -- ideal for sports and other odds and ends 


# patches

Font.xml

in the Default fontset

```xml
<font>
  <name>font8_poster</name>
  <filename>Roboto-Thin.ttf</filename>
  <size>16</size>
  <style>bold</style>
  <linespacing>0.85</linespacing>
</font>
```

strings.po

```
#. viewtype name
msgctxt "#31990"
msgid "Poster Files"
msgstr "Poster Files"
```

MyVideoNav.xml

1. add 560 to `views`

```xml

	<views>50,51,52,53,54,55,500,501,502,560</views>

```

2. add in the `include`

```xml
<include>View_560_PosterFiles</include>
```
