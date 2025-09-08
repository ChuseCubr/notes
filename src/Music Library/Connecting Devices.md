When syncing between devices using [[Syncthing]], both devices must add the other in order for them to communicate.

> [!NOTE]+
> The service must be running on both devices for this to work.
>
> To ensure that the service is running:
>
> - On Windows, ensure that [[Syncthing]] is running by visiting [http://localhost:8384](http://localhost:8384) in your browser. If it is not running, you can manually run it through the Windows start menu. Don't be alarmed, this will bring up a terminal.
> ![[Syncthing#^autostart]]
> - On iOS, you must have [[Syncthing#iOS|Möbius Sync]] open.
> - On Android, you must have [[Syncthing#Android|Syncthing-Fork]] open.

^running-syncthing

## Windows and iOS

1. Take note of the device ID:
    1. Open the `actions` dropdown (gear icon, top right corner)
    2. Click `show ID`
2. Add the other device:
    1. Click `add remote device`
    2. Fill in the `device ID` with the ID of the other device
    3. Fill in the `device name` however you want
    4. Click `save`

## Android

1. Take note of the device ID:
    1. Open the sidebar
    2. Click `show device ID`
2. Add the other device:
    1. Navigate to the `devices` tab
    2. Tap the icon in the top right
    3. Fill in the device ID with the ID of the other (optionally, you make scan the QR code)
    4. Fill in the name however you want
    5. Tap the check icon in the top right

