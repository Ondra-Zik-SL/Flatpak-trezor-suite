# Flatpak-trezor-suite
Proof of concept for runing trezor sutie as fletpak app.

clone this repository

build the app with flatpak builder
``flatpak-builder --force-clean --user --install-deps-from=flathub --repo=repo --install builddir io.trezor.suite.yml``

run the flatpak with:
``flatpak run io.trezor.suite``
