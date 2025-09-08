There is where, within the file system, you can dump albums for [[Library Setup#MusicBee]] to import. When scanned, the files and folders here will be moved to and sorted within the [[Library Folder]].

You can scan this folder for new files [[#Scanning Manually|manually]], or set it up to be [[#Scanning on Startup|scanned on startup]].

> [!IMPORTANT]+
> The folder must already exist. If it doesn't yet, create it before proceeding with the next instructions.

>[!WARNING]+
> The inbox folder is automatically cleaned up after scanning. However, if the folder will become empty after importing files, the folder itself will be deleted. To prevent this, you can add an empty text file within the folder.

## Scanning Manually

1. Press `insert` on the keyboard to open the `scan folders for new files` dialog
2. Configure the inbox folder(s)
    1. In the top right corner, click `choose folders`
    2. Navigate and select the folders you wish to be your inbox folder
    3. Click `ok`
3. Ensure `add to library` is selected
4. Click `proceed` to scan for new files

## Scanning on Startup

1. Navigate to the `monitored folders` settings
    1. Press `ctrl+o` on the keyboard to open the `preferences` dialog
    2. In the sidebar, click `library`
2. Configure the inbox folder(s)
    1. Click `choose folders`
    2. Navigate and select the folders you wish to be your inbox folder
    3. Click `ok`
3. Enable `scan on startup` (continuous monitoring is a little janky in my experience)
4. Click `apply` then `save`
