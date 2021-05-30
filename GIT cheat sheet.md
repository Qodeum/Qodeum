# GIT CHEAT SHEET

### Frequently used commands
- To initialize GIT repo for working directory
`$ git init `
- Add files from working directory
`$ git add . `
- Commit ALL changes from working directory to GIT repo
`$ git commit -all -m "userful commit message here" `
- Push to GIT repo upstream, after code commit
`$ git push -all -u `

### GIT create
- Create a brand new GIT enabled project folder in working directory
`$ git init new-project-name-here `

### GIT clone
- Clone an existing GIT url
`$ git clone existing-git-url-here `

### GIT verify
- Get GIT status for the working directory
`$ git status `

### GIT compare
- Get list of uncommited changes since last commit
`$ git diff `
- Compare file in working directory against GIT HEAD
`$ git diff ./file_path `
OR
`$ git git diff HEAD ./file_path `
- Compare two GIT branches
`$ git diff branch_one..branch_two `

### GIT history
- Get version history for current GIT branch
`$ git log `
- Get version history for a specific file on current GIT branch
`$ git log -follow file `
