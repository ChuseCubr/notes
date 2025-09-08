Ideally, the library would be a collection of [FLAC](https://en.wikipedia.org/wiki/FLAC) files, which retain the highest available quality. However, this would take up a significant amount of storage. To limit the use of storage for syncing on smaller devices, you can reencode them into more space efficient lossy file formats.

# Encoder

[[Library Setup#MusicBee]] has built-in functionality for automatically converting across different file formats. For the purpose of this tutorial, I will be using [Opus](https://en.wikipedia.org/wiki/Opus_(audio_format)). However, MusicBee does not come with an Opus encoder, so you will need to install the [encoder pack](https://getmusicbee.com/addons/plugins/364/encoder-pack/).

> [!TIP]+
> MusicBee's default maximum quality setting for Opus is overkill. I would recommend making it a little less over kill at [192 kbps](https://wiki.hydrogenaudio.org/index.php?title=Opus#Bitrate_performance). To do this:
>
> 1. Open the `preferences` dialog by pressing `ctrl+o`
> 2. Navigate to the `file converters` tab
> 3. Scroll down and enable the `opus` converter
> 4. Verify that it is using the encoder you installed (should be `OpusEnc.exe`)
> 5. Set the `bitrate` in the `maximum quality` setting to `192`

# Virtual Device

MusicBee can automatically convert files when syncing with a device. However, I find this kind of file transfer between Windows and mobile devices finicky. Instead, I recommend creating a virtual device that represents a folder and syncing that folder using [[Syncthing]].

To set up a virtual device with reencoding:

1. Press `ctrl+o` to open the `preferences` dialog
2. Navigate to the `devices` tab
3. Choose the folder for the virtual devices
    1. Click `add virtual device...`
    2. Navigate to and select the folder you wish to save your reencoded library to
    3. Click `ok`
4. Configure the virtual device
    1. In the `music` tab, ensure `synchronize music` and `all music` are selected
    2. Navigate to the `on-the-fly conversion` section under the `settings` tab
    3. Check `convert to:`
    4. Select `opus` (if you do not see this option, see [[#Encoder]])
    5. Under `encoding profile`, select either `high quality` or `maximum quality` (see why [here](https://wiki.hydrogenaudio.org/index.php?title=Opus#Bitrate_performance))
    6. Select `only convert files with a lossless format` to avoid [generation loss](https://en.wikipedia.org/wiki/Generation_loss)
    > [!TIP]+ For consistency across your library, I also recommend the following settings:
    >
    > 1. At the top, select `delete files that are not on the auto-sync list from the device`
    > 2. Under `media storage`:
    >     1. Select `use naming template`
    >     2. Ensure that the `music files` template is same as in your [[Library Folder]] auto-organize template (`<Album Artist>\\<Album>\\<Disc-Track#> - <Title>` by default)
5. Click `save`

