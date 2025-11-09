# keyd-config
My [keyd](https://github.com/rvaiya/keyd) config for [Fedora](https://fedoraproject.org) on HP Envy x360 2-in-1 Laptop 16-ac0xxx

## Features

- My config fixes the behaviour that moving the screen on a HP Envy x360 2-in-1 Laptop 16-ac0xxx activates aeroplane mode in Fedora
  - See https://www.reddit.com/r/linux/comments/1d9c2fr/a_quick_guide_to_linux_on_the_hp_envy_x360_2in1/ for more details
- Adds the keyboard shortcut `ctrl+shift+a` to open right-click menus

## Installation

1. Clone this repository
```bash
git clone https://github.com/Christopher-K-Long/keyd-config
```
2. Install [keyd](https://github.com/rvaiya/keyd)
```bash
git clone --depth=1 https://github.com/rvaiya/keyd
cd keyd
make && sudo make install
sudo systemctl enable keyd && sudo systemctl start keyd
```
3. Copy config
```bash
cd keyd-config
sudo cp default.conf /etc/keyd/default.conf
```
4. Restart keyd
```bash
sudo keyd reload
```

### As a single bash script
```bash
# 1. Clone this repository
git clone https://github.com/Christopher-K-Long/keyd-config

# 2. Install keyd
git clone --depth=1 https://github.com/rvaiya/keyd
cd keyd
make && sudo make install
sudo systemctl enable keyd && sudo systemctl start keyd

# 3. Copy config
cd keyd-config
sudo cp default.conf /etc/keyd/default.conf

# 4. Restart keyd
sudo keyd reload
```
