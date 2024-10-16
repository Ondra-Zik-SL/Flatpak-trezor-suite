
# Flatpak-trezor-suite
Trezor Suite as a Flatpak app.

### Install:

Install flatpak builder

    flatpak install -y flathub org.flatpak.Builder

You may need to add the Flathub repository for your user.

    flatpak remote-add --user --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo

Clone this repository

    git clone https://github.com/Ondra-Zik-SL/Flatpak-trezor-suite.git

Build the app with flatpak builder

    flatpak run org.flatpak.Builder --force-clean --sandbox --user --install-deps-from=flathub --ccache --mirror-screenshots-url=https://dl.flathub.org/media/ --repo=repo builddir io.trezor.suite.yml
Add the local Flatpak repository.

    flatpak remote-add --user --no-gpg-verify my-app file://$(pwd)/repo

Install the Trezor Suite from the local repository.

    flatpak install --user -y my-app io.trezor.suite

Run the flatpak with.

    flatpak run io.trezor.suite
