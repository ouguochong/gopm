gpm - Go Package Manager
===

![GPMGo_Logo](https://raw.github.com/GPMGo/gpm-site/master/static/img/gpmgo2.png?raw=true)

gpm(Go Package Manager) is a Go package manage tool for search, install, update and share packages in Go.

## Main commands

- `build` compiles and installs packages and dependencies: basically, it calls `go install` and moves executable to current path from `GOPATH` if any, the executable name is the folder name which is default by `go install`.
- `install` downloads and installs packages and dependencies: you can download packages without version control tools like git, hg, svn, etc. It downloads and installs all packages including all dependencies automatically(except when you use bundle or snapshot id). For now, this command supports `code.google.com`, `github.com`, `launchpad.net`, `bitbucket.org`. 

## Todo

- Command `remove` is for removing packages.
- Add gpm working principle design.
- Add support for downloading tarballs from user sources.
- After downloaded all packages in bundles or snapshots, need to check if all dependencies have been downloaded as well.
- Develop user source API server template application to support user sources in bundles.
- Add bundle and snapshot parser code for downloading by bundle or snapshot id.
- Add user system to create, edit, upload, and download bundles or snapshots through gpm client program.
- Download package from code.google.com only support hg as version control system, probably support git and svn.
- Add support for downloading by tag and branch for packages in bitbucket.org, git.oschina.net, gitcafe.com.
- Collect download and installation results and report to users in the end.
- Command `install` add support for downloading code from git.oschina.net, gitcafe.com, *.codeplex.com;
- Command `check` is for checking and downloading all missing dependencies.
- Command `daemon` is for auto-compile web applications when debug it locally.
- Command `update` is for checking updates.
- Command `search` is for searching packages.
- Add feature "struct generator".
- i18n support for Chinese.
- Add built-in application version in order to backup data when users update.
