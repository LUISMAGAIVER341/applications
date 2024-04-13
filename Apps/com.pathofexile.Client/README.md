# Path of Exile
Path of Exile is an online Action RPG

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | Yes      | Yes  | Slight stuttering when entering new areas |
| 64bit | Yes      | Yes  | Slight stuttering when entering new areas |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak com.pathofexile.Client.yml
    flatpak --user install winepak com.pathofexile.Client
    
#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak com.pathofexile.Client.yml
    flatpak --user install winepak com.pathofexile.Client

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds com.pathofexile.Client.yml
    
#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds com.pathofexile.Client.yml

## Run

    flatpak run com.pathofexile.Client

