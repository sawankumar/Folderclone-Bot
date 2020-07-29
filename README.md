<h1 align="center">FolderClone 🔥</h1> 

<p align="center">
<a href="https://github.com/sawankumar"><img alt="author" src="https://img.shields.io/badge/author-Sawan%20Kumar-red"/></a>
<a href="https://www.python.org/"><img alt="language" src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg"/></a>
<a href="https://github.com/ellerbrock/open-source-badges/"><img alt="author" src="https://badges.frapsoft.com/os/v1/open-source.svg?v=103"/></a>
</p>

<hr>


> ## FolderClone: A project that allows you copy large folders to Shared Drives.

## Usage
1. Follow [instructions](https://github.com/sawankumar/AutoRclone) and create service accounts.
2. Copy the .json files to **accounts** folder.
3. Edit the values in `config.py`.
5. Run `py folderclone.py`.

## Deploy on Heroku
1. Clone this repository.
2. Inside this repository make a folder and name it `accounts`.
3. Create your service accounts and add it in `accounts` folder.
4. Edit the values in `config.py`.
5. Push the files to your github repository.
6. Use `Deploy To Heroku Button`

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/sawankumar/FolderClone-Bot/tree/master)


## Usage in telegram bot
`/folderclone <source_id> <dest_id> <thread>`

`source_id` - Drive ID of the folder you want to copy from. (Required)

`dest_id` - Drive ID of the folder you want to copy into. (Required)

`thread` - Amount of threads to use. The higher the more resource it requires. Default - 25

## BotFather Commands

```
- folderclone - Clones Folder From SRC to DST
- status - Shows Current Ongoing Progress
- uptime - Bot Uptime
- stop - Stops Ongoing Progress
```

## Customize 
- Set thread number by changing values at `line 43` in `clonerbot.py`.

- Customize clone command by changing command at `line 171` in `clonerbot.py`.

## Concerning thread number
- Recommended thread number for heroku is 25.

- 40 will cause occasional RAM over usage and stall the app.
  
- 50 if you want to risk your app hanging.
  
- Anything above 50 will more likely crash the app.

### Note
- `folderclone.py` - Modified version of `multifolderclone.py` from [Folderclone](https://github.com/Spazzlo/folderclone).

- Commits  Merged Till `Jul 29, 2020` [450eae3](https://github.com/Loli-Killer/TgFolderClone/commits/master) from [TgFolderClone](https://github.com/Loli-Killer/TgFolderClone)

