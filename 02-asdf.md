# ASDF

## [Installation](https://asdf-vm.com/guide/getting-started.html)

- [Step 1](https://asdf-vm.com/guide/getting-started.html#_1-install-dependencies): Check whether `git` and `curl` are
  installed
- [Step 2](https://asdf-vm.com/guide/getting-started.html#_2-download-asdf): Download
  asdf `git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.14.0`
- [Step 3](https://asdf-vm.com/guide/getting-started.html#_3-install-asdf): Install asdf, add `. "$HOME/.asdf/asdf.sh"` and `. "$HOME/.asdf/completions/asdf.bash"` to `~/.bashrc`
- [Step 4](https://asdf-vm.com/guide/getting-started.html#_4-install-a-plugin): Install plugins
  - Node
    - No plugin dependencies to install
    - `asdf plugin add nodejs https://github.com/asdf-vm/asdf-nodejs.git`
    - `asdf install nodejs 20.15.0`
    - `asdf global nodejs 20.15.0`
  - PNPM
    - No plugin dependencies to install
    - `asdf plugin add pnpm`
    - `asdf install pnpm 9.4.0`
    - `asdf global pnpm 9.4.0`
  - Java
    - All plugin dependencies installed by default
    - `asdf plugin-add java https://github.com/halcyon/asdf-java.git`
    - `asdf install java temurin-21.0.3+9.0.LTS`
    - `asdf global java temurin-21.0.3+9.0.LTS`
    - Set JAVA_HOME: add `. $HOME/.asdf/plugins/java/set-java-home.bash` to `~/.bashrc`