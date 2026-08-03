# 💻 Mac Basic Setup
> Thing todo for a new Mac

### 📱 Apps
- Terminal: [Ghossty]([https://iterm2.com/](https://ghostty.org/))
- Browser: [Dia](https://www.diabrowser.com/release-notes/latest)
- Screensaver settings: [Jolt](https://apps.apple.com/kr/app/jolt-of-caffeine/id1437130425?mt=12)
- [Postman](https://www.postman.com/downloads/)

### 🛠️ Setups
- **homebrew**: [official link](https://brew.sh/ko/)
  ```bash
  # check homebrew installation
  brew -v

  # install homebrew
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  ```
- **oh-my-zsh**: [ref](https://stdhsw.tistory.com/102)
  ```bash
  # install oh-my-zsh
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

  # download auto-complete plugin
  git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
  git clone https://github.com/zsh-users/zsh-syntax-highlighting ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

  # add plugin
  # fix to: plugins=(git zsh-syntax-highlighting zsh-autosuggestions)
  vi ~/.zshrc

  # download p10k theme
  git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

  # set theme
  # fix to: ZSH_THEME="powerlevel10k/powerlevel10k"
  vi ~/.zshrc
  ```
  <!-- vscode와 iTerm2 연동하기
  vscdoe와 iTerm2를 연동하기 위해 vscode를 실행하고 설정(cmd + ,)으로 들어가 "External: Osx Exec"를 검색하여 "iTerm.app"을 입력해주면 됩니다. -->
