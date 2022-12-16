## Privileges
- Not all users can run all commands
	- Some are for Administrator only
- Standard privileges
	- Runs as normal user
	- Works for most commands
- Administrative/elevated privileges
	- Must be part of Administrators group
	- Right click Command prompt -> Run as Administrator
	- Type `cmd` in search -> Ctrl+Shift+Enter
## Command Line Troubleshooting
- Use `help`
	- `help dir`
	- `help chkdsk`
- `[command] /?`
- To close type `exit`
## File Management
- `dir`
	- List files and directories
- `cd` or `chdir`
	- Chance working directory
	- `\` to specify between folders
- `..` to go up one folder
- `mkdir`, `chdir`, `rmdir`
	- Make / Change / Remove directory
	- Can be shortened to `md`, `cd`, `rd`
## Drive Letters
- Each drive gets a letter 
- Primary drive is usally `C:`
## hostname
- `hostname` lets us view name of device
- Windows Device name
- Can be changed in system settings
## format
- `format` command formats a disk to use with Windows
- Can lose data if not careful
## copy
- `copy`
- `/v` verifies it is written correct
- `/y` suppress prompts
## xcopy
- Multiple files and directories
- `xcopy /s <source> <destination>`
## Robust Copy
- `robocopy`
- A better `xcopy`
	- More features
	- 
- Windows 10 and 11
## shutdown
- `shutdown /s /t nn`
	- Shutdown
	- `nn` is delay in seconds
- `shutdown /r /t nn`
	- Restart
- `shutdown /a`
	- Abort shutdown
## DiskPart
- `diskpart`
- Manage disk configurations
	- Disks, partitions, volumes
- Can lose data if not careful
## winver
- `winver`
- About info for Windows
- Useful for troubleshooting
## Managing Group Policy
- Manage computers in AD
- Group Policy is updates at login
- `gpupdate`
	- Force GP update (won't have to re-login)
	- `gpupdate /targe:{computer|user} / force`
- `gpresult`
	- Verify policy settings for cumputer or user
	- `gpresult /r`
	- `gpresult /user sgc/professor /v`
