# sap-avatar-grab
Grab avatars from SAP

On your SAP page of choice, paste the following command in the URL bar:
```
javascript:{let avatarImageHolder = document.querySelector(".sapFAvatarImageHolder.sapFAvatarImageCover"); let found = /url\(['"]?(.*?)['"]?\);?/g.exec(avatarImageHolder.style.backgroundImage); window.open(found[1], '_blank').focus();}
``` 

Your operating system/browser may omit the javascript: prefix. Please make sure this prefix is also copied, else the code will not be executed.