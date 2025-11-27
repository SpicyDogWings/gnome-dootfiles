# GNOME .files
Esto es un repo de gnome con los archivos necesarios para una instalación limpia en fedora 43
## Requisitos
Primero se deben instalar las siguientes dependencias de los repos oficiales
``` bash
dnf install zsh git
```
Tambien para una correcta integración puedes instalar `ohMyZsh` en el sistema para instalar una gran cantidad de plugins. Y para 2 buenos plugins como son el completions y el syntax puedes descargarlos con
``` bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
Además es recomendable instalar `rust` con `cargo` e instalar `cargo-binstall`
``` bash
cargo install cargo-binstall
```
Las dependencias de `rust` son
``` bash
cargo binstall eza
```
## Instalación
``` bash
chezmoi init --apply https://github.com/SpicyDogWings/gnome-dootfiles.git
```