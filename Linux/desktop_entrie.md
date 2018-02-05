# Add desktop entrie

> Discord is used as exemple

#### Application entrie

Under 
```
~/.local/share/applications
```
Add the `.desktop` (Discord exemple)

```
[Desktop Entry]
Name=Discord
StartupWMClass=discord
Comment=All-in-one voice and text chat for gamers
GenericName=Internet Messenger
Exec=/usr/share/discord/Discord
Icon=discord
Type=Application
Categories=Network;InstantMessaging;
```

#### Icons

Make or go to
```
~/.icons
```
The `Icon` line should be in the form of `Icon=<icon.png>`, with just 
the file name (including the extension), no directory information.
