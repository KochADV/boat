# Local DEV Environment

## Tool Configuration
### LaRavel via Docker + Sail in Windows
- LaRavel Documentation: https://laravel.com/docs/11.x/installation#sail-on-windows
- be sure to start ubunut by:
    - Opening Windows Powershell
    - Click "down arrow" in top menu
    - Select "Ubuntu"
#### WSL (Windows Linux SubSystem)
- Install: https://learn.microsoft.com/en-us/windows/wsl/install
- Username under "Keeper - WSL UNIX Username"

#### Docker Desktop
- https://www.docker.com/products/docker-desktop/
- Configure DockerDesktop to use WSL: https://docs.docker.com/desktop/features/wsl/
    - Note you have to update "settings>General" checkbox AND "settings>Resources>WSL Integration"
    - See Gios Video here: https://www.youtube.com/watch?app=desktop&v=4K4nkncZ2OQ

### Launch Sail
- Run
```
./vendor/bin/sail up -d" in Ubuntu Powershell (-d runs in background)
```

### Open project in conatiner with VS Code
- click File>Open Folder
- Open from this location:  
```
     \\wsl.localhost\Ubuntu\home\merwester74
```
- type localhost into browser
    - if there is an error try running migration:  ./vendor/bin/sail artisan migrate
