Once [[Connecting Devices|devices are connected]] within [[Syncthing]], you can start syncing folders.

![[Connecting Devices#^running-syncthing]]

> [!IMPORTANT]+
> The folder must already exist. If it doesn't yet, create it before proceeding with the next instructions.

> [!TIP]- Shrinking large libraries
> If your library consists of [FLAC](https://en.wikipedia.org/wiki/FLAC) files, and you are syncing to a device with storage constraints (like a phone), I would recommend [[Reencoding]] to save space.
>
> If you do so, follow the next instructions with the folder your [[Reencoding#Virtual Device]] is pointing to.

# On Windows

As this guide is about managing your music library with MusicBee, this part of the guide assumes that you'd like to sync your files from a Windows device.

1. Click `add folder`
2. In the `general` tab:
    1. Fill in the `folder label` however you want
    2. Take note of the `folder ID`
    3. Fill in the path with the path to your library (or path to your [[Reencoding#Virtual Device]], if you set up [[Reencoding]])
3. In the `sharing` tab:
    1. Select the device you'd like the sync to
4. Click `save`

# On the Other Device

Following the previous instructions, the device you selected should receive a notification for syncing a folder. Tap that, and navigate to and select the folder you'd like your library to be located in.

If you did not receive a notification, you'll have to set it up manually:

1. Click `add folder`
    - On iOS, this will be in the same position as on Windows
    - On Android, it will be in the top right corner of the `devices` tab
2. In the `general` tab:
    1. Fill in the `folder label` however you want
    2. Replace the `folder ID` with the ID you noted earlier
    3. Fill in the path you'd like to save the library
3. Click `save`
