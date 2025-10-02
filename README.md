### mobile-config-firefox flatpak extension

build

```sh
flatpak run org.flatpak.Builder --user --install --install-deps-from=flathub --force-clean --repo=repo build org.mozilla.firefox.systemconfig.yml
```

install

```sh
sudo flatpak remote-add pocketblue https://pocketblue.github.io/pocketblue.flatpakrepo
flatpak install pocketblue org.mozilla.firefox.systemconfig
```

uninstall

```sh
flatpak remove org.mozilla.firefox.systemconfig
gio trash ~/.var/app/org.mozilla.firefox/.mozilla/firefox/*/chrome
```
