# Safe checklist: removing smart-TV ads with Claude Code

Based on the public cleanyourtv and dumbtv projects (reported by TechCrunch, Oct 19 2026). Do this at your own risk. One user bricked their TV.

1. **Check your TV.** This only works on Android TV and Google TV. Samsung (Tizen) and LG (webOS) are not supported.
2. **Turn on developer options.** Settings → About → click "Build" 7 times, then turn on USB / network debugging (ADB).
3. **Use the same Wi-Fi.** Run Claude Code on a computer on the same network as the TV.
4. **Back up first.** Ask Claude to save the full package list (`adb shell pm list packages > backup.txt`) and write a `restore.sh` that turns everything back on.
5. **Disable, don't uninstall.** Use `pm disable-user`, so every change can be undone. No root needed.
6. **Go slowly.** Switch off ad, telemetry and ACR (viewing-tracking) services in small batches, and reboot to test after each batch.
7. **Never touch system-critical packages** (setup wizard, input/HDMI services, the package installer, or the stock launcher until a new one is set as default).
8. **Install a clean launcher** (e.g. Projectivy, FLauncher or ATV Launcher) and set it as the default home screen.
9. **If something breaks,** run `restore.sh`. If that fails, a factory reset brings back the stock setup.

Source projects: github.com search "cleanyourtv" and "dumbtv". Both are works in progress.
