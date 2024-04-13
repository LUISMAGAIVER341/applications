# Overwatch
Competitive 6v6 team objective FPS

## Status

| Arch  | Installs | Runs | Notes |
| ----- | -------- | ---- | ----- |
| 32bit | N/A      | N/A  | No 32bit client available |
| 64bit | Yes      | Yes  | Game runs with occasionally stuttering, with a RX 480 an average of 40~50 FPS with drops to 30 FPS |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak com.blizzard.Overwatch.yml
    flatpak --user install winepak com.blizzard.Overwatch

#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak com.blizzard.Overwatch.yml
    flatpak --user install winepak com.blizzard.Overwatch

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds com.blizzard.Overwatch.yml

#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds com.blizzard.Overwatch.yml

## Run

    flatpak run com.blizzard.Overwatch

