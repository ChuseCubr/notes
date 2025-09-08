This page is only for installing the syncing software. To set it up for our purposes, see [[Sync Setup]].

[Syncthing](https://syncthing.net) is a tool used to sync folders between devices across networks.

# Windows

In my opinion, the easiest way to install Syncthing is through [Scoop](https://scoop.sh).

To check if you have Scoop installed, open PowerShell and run the following:

```powershell
scoop --version
```

If you get an error, install scoop by running the following:

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

After ensuring Scoop installed, use it to install Syncthing:

```powershell
scoop install syncthing
```

> [!TIP]+ Autostart
> You can set Syncthing to run on startup following [these instructions](https://docs.syncthing.net/users/autostart.html), using the file returned from running:
>
> ```
> scoop which syncthing
> ```

^autostart

# Android

The official Syncthing Android app has been [discontinued](https://docs.syncthing.net/users/autostart.html).

You can download a fork maintained by the community [here](https://play.google.com/store/apps/details?id=com.github.catfriend1.syncthingandroid&hl=en).

# iOS

There is no official Syncthing iOS app, but there is [Möbius Sync](https://apps.apple.com/us/app/m%C3%B6bius-sync/id1539203216?ign-itscg=30200&ign-itsct=apps_box), which is a Syncthing wrapper.
