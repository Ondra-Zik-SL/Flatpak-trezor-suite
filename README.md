
# Flatpak-trezor-suite
Proof of concept for running Trezor Suite as a Flatpak app.

clone this repository

    git clone https://github.com/Ondra-Zik-SL/Flatpak-trezor-suite.git

You may need to add the Flathub repository for your user.

    flatpak remote-add --user --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo


build the app with flatpak builder

    flatpak-builder --force-clean --user --install-deps-from=flathub --repo=repo --install builddir io.trezor.suite.yml

run the flatpak with:

    flatpak run io.trezor.suite
