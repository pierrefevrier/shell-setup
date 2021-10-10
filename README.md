# Shell Setup

## MacOS

### 

### Homebrew
- Gestionnaire de paquets de MacOS
- Suivre les instructions suivantes : https://brew.sh/index_fr

### ZSH
- Déjà installé avec les dernières release de MacOS

### Oh My Zsh
- Pour personnaliser ZSH via un ensemble de plugins (liste dispo ici : https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins)
- Suivre les instructions suivantes : https://ohmyz.sh/#install

### iTerm2
- La liste des features : https://iterm2.com/features.html
  - Killing feature : supporte par défaut le thème Dark Solarized (ce qui n'est pas la cas du terminal par défaut sur MacOS)
- Installer via homebrew : `brew cask install iterm2`
- Installer le thème `agnoster`(suivre le chapitre #todo)
  - Pour que l'affichage soit correct (la barre du path dans le prompt), aller dans les préférences de iTerm
    - `Profiles > Default > Text > Font` : `Meslo LG M for Powerline`
  - Pour activer le thème Dark Solarized (couleurs douces dans le terminal), aller dans les préférences de iTerm
      - `Profiles > Default > Colors > Color Presets...` : `Solarized Dark`

## Commun

### Oh My Zsh
- Thème agnoster (permet notamment de colorer le path du prompt)
  - Basculer sur le thème `agnoster` en suivant les instructions suivantes : https://github.com/ohmyzsh/ohmyzsh#selecting-a-theme
  - Au départ, l'affichage ne sera pas bon, normal, il faut installer en plus les `Powerline fonts` en suivant les instructions suivantes : https://medium.com/featurepreneur/how-to-apply-agnoster-theme-in-mac-zshrc-876f3baf8bf
    - Le repo des polices peut être supprimé une fois qu'elles sont installées sur le système
    - Utiliser la police `Meslo LG M for Powerline` dans les terminaux pour que l'affichage soit correct
      - `M` : c'est pour la taille de l'interline
      - `DZ` : c'est pour configurer la manière dont doit s'afficher le `O` (plus d'infos : https://github.com/ryanoasis/nerd-fonts/issues/190)
        - `DZ` = avec un `/` au milieu du `0`
        - sans `DZ` = avec un `.` au milieu du `0`
  - Virer le username du prompt
    - Ajouter les lignes suivantes en fin de fichier `.zshrc` :
    ```
    # hide the username
    DEFAULT_USER prompt_context(){}
    ```
