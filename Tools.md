### 工欲善其事必先利其器



| What For | Tool Name |      |
| -------- | --------- | ---- |
|          |           |      |
|          |           |      |
|          |           |      |



## GoLand

`Golang`

license server address栏中输入下面服务器地址

<http://intellij.mandroid.cn/>，然后点击OK就可以了。 

<http://idea.imsxm.com/> 
<http://idea.iteblog.com/key.php>

## DataGrip

`Data Base`

```powershell
$ sudo apt-get update
$ sudo apt-get install datagrip
```

# [Datagrip 2017.2 激活](http://www.cnblogs.com/li1234yun/p/7967843.html)

## 解决方法

参考网址：<https://jetbrains-server.ru/2017/03/31/datagrip-2016-2017-activation/page/2/>

亲测使用`http://idea.imsxm.com/`通过`license server`方式联网可以进行激活。

## pip

（1）下载pip

进入https://pypi.python.org/pypi/pip，下载第二项。
pip-9.0.1.tar.gz (md5, pgp)

（2）解压安装

解压下载的文件（windows下只用解压工具解压如RAR，Linux下终端输入tar -xf pip-9.0.1.tar.gz，即tar -xf 文件名），进入解压后的文件夹中，调出命令行窗口或者终端，windows下输入

python setup.py install
1
Linux下输入

sudo python setup.py install
1
安装成功后测试下，输入

pip -v
1
搞定！

## oh-my-zsh
## Getting Started

### Prerequisites

__Disclaimer:__ _Oh My Zsh works best on macOS and Linux._

* Unix-like operating system (macOS or Linux)
* [Zsh](http://www.zsh.org) should be installed (v4.3.9 or more recent). If not pre-installed (`zsh --version` to confirm), check the following instruction here: [Installing ZSH](https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH)
* `curl` or `wget` should be installed
* `git` should be installed

### Basic Installation

Oh My Zsh is installed by running one of the following commands in your terminal. You can install this via the command-line with either `curl` or `wget`.

#### via curl

```shell
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

#### via wget

```shell
sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```

## Using Oh My Zsh

### Plugins

Oh My Zsh comes with a shitload of plugins to take advantage of. You can take a look in the [plugins](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins) directory and/or the [wiki](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins) to see what's currently available.

#### Enabling Plugins

Once you spot a plugin (or several) that you'd like to use with Oh My Zsh, you'll need to enable them in the `.zshrc` file. You'll find the zshrc file in your `$HOME` directory. Open it with your favorite text editor and you'll see a spot to list all the plugins you want to load.

```shell
vi ~/.zshrc
```

For example, this might begin to look like this:

```shell
plugins=(
  git
  bundler
  dotenv
  osx
  rake
  rbenv
  ruby
)
```

#### Using Plugins

Most plugins (should! we're working on this) include a __README__, which documents how to use them.

### Themes

We'll admit it. Early in the Oh My Zsh world, we may have gotten a bit too theme happy. We have over one hundred themes now bundled. Most of them have [screenshots](https://wiki.github.com/robbyrussell/oh-my-zsh/themes) on the wiki. Check them out!

#### Selecting a Theme

_Robby's theme is the default one. It's not the fanciest one. It's not the simplest one. It's just the right one (for him)._

Once you find a theme that you'd like to use, you will need to edit the `~/.zshrc` file. You'll see an environment variable (all caps) in there that looks like:

```shell
ZSH_THEME="robbyrussell"
```

To use a different theme, simply change the value to match the name of your desired theme. For example:

```shell
ZSH_THEME="agnoster" # (this is one of the fancy ones)
# see https://github.com/robbyrussell/oh-my-zsh/wiki/Themes#agnoster
```

_Note: many themes require installing the [Powerline Fonts](https://github.com/powerline/fonts) in order to render properly._

Open up a new terminal window and your prompt should look something like this:

![Agnoster theme](https://cloud.githubusercontent.com/assets/2618447/6316862/70f58fb6-ba03-11e4-82c9-c083bf9a6574.png)

In case you did not find a suitable theme for your needs, please have a look at the wiki for [more of them](https://github.com/robbyrussell/oh-my-zsh/wiki/External-themes).

If you're feeling feisty, you can let the computer select one randomly for you each time you open a new terminal window.


```shell
ZSH_THEME="random" # (...please let it be pie... please be some pie..)
```

And if you want to pick random theme from a list of your favorite themes:

```shell
ZSH_THEME_RANDOM_CANDIDATES=(
  "robbyrussell"
  "agnoster"
)
```

# Powerline fonts

This repository contains pre-patched and adjusted fonts for usage with the [Powerline](https://github.com/powerline/powerline) statusline plugin.

## Installation

Run `./install.sh` to install all Powerline Fonts or see the [documentation](https://powerline.readthedocs.org/en/latest/installation/linux.html#fonts-installation) for details.

## Quick installation

If you are running a Debian or Ubuntu based Linux distribution, there should be a package available to install the Powerline Fonts with the following command:

```
sudo apt-get install fonts-powerline

```

On other environments, you can copy and paste these commands to your terminal. Comments are fine too.

```
# clone
git clone https://github.com/powerline/fonts.git --depth=1
# install
cd fonts
./install.sh
# clean-up a bit
cd ..
rm -rf fonts

```

## Uninstall

Run `./uninstall.sh` to uninstall all Powerline Fonts. You can also copy the quick installation commands changing only the line `./install.sh` to `./uninstall.sh`.

In both cases, please make sure you are working with the exact same version of Powerline fonts you had checked out while installing.



## Fonts installation

### Fontconfig

https://powerline.readthedocs.io/en/latest/installation/linux.html#fonts-installation

This method only works on Linux. It’s the second recommended method if terminal emulator supports it as patching fonts is not needed, and it generally works with any coding font.

1. Download the latest version of the symbol font and fontconfig file:

   ```
   wget https://github.com/powerline/powerline/raw/develop/font/PowerlineSymbols.otf
   wget https://github.com/powerline/powerline/raw/develop/font/10-powerline-symbols.conf

   ```

2. Move the symbol font to a valid X font path. Valid font paths can be listed with `xset q`:

   ```
   mv PowerlineSymbols.otf ~/.local/share/fonts/

   ```

3. Update font cache for the path the font was moved to (root priveleges may be needed to update cache for the system-wide paths):

   ```
   fc-cache -vf ~/.local/share/fonts/

   ```

4. Install the fontconfig file. For newer versions of fontconfig the config path is `~/.config/fontconfig/conf.d/`, for older versions it’s `~/.fonts.conf.d/`:

   ```
   mv 10-powerline-symbols.conf ~/.config/fontconfig/conf.d/
   ```