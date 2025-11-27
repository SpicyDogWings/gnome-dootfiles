# GNOME .files
Esto es un repo de gnome con los archivos necesarios para una instalación limpia en fedora 43
## Requisitos
Primero se deben instalar las siguientes dependencias de los repos oficiales
``` bash
dnf install zsh git
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