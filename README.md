# Git-GUI-ultra-simple-password-manager
Best Git-GUI password manager , password storage and helper. No complicated configurations required. No strange foreign binaries required. Portable-way storage.

### Installation

> 1) find `git-gui--askpass` file in your Git installation path (in `C:\Git\mingw64\libexec\git-core\` or something with your installation path)
> 2) overwrite or edit `git-gui--askpass`
> 3) Ready to use!
> 

### What has been added?

Added block for login insertion as text, directly from code:
```
if {[string match "{Username *}" $argv]} {
	set answer "edit_to_place_email_here_used_as_login@your_email.ru"
}
```

Added block for password insertion as text, directly from code:
```
if {[string match "{Password for *}" $argv]} {
	set answer "edit_to_place_passowrd_here_used_as_password_for_git_repos_server"
}
```
Modified caption/name of window, to provide user understanding of what is happening: 
```
wm title . "OpenSSH_Edit_to_place_here_profile_name_to_identify_action"
```
