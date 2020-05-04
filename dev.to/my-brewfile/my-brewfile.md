I am a big fan of using [Homebrew](https://brew.sh) to install/update all the software on my MacBook. One thing that not everyone knows about is the idea of a [`Brewfile`](https://github.com/Homebrew/homebrew-bundle), which is a text file that lists all the various packages, etc, and you can then use `brew bundle` to install the things in the `Brewfile` (along with their dependencies). Brewfiles support more than just Homebrew packages; you can use a `Brewfile` to list out casks, as well as apps installed from the Mac App Store.

My current `Brewfile` is [available on GitHub](https://github.com/mattstratton/matty-dotfiles/blob/master/Brewfile), but I thought it might be helpful to go through it and provide some explanation of each package/application, and what I use them for.

## Packages

This is not a comprehensive list of all the packages I have installed, but just some that you might wonder about!

- [asciinema](https://formulae.brew.sh/formula/asciinema): Record what you do in a terminal! Fancy!
- [autojump](https://formulae.brew.sh/formula/autojump): Little fun tool to make it easier to [jump to a different directory](https://github.com/wting/autojump).
- [diff-so-fancy](https://formulae.brew.sh/formula/diff-so-fancy): Make your [diffs look cooler ](https://github.com/so-fancy/diff-so-fancy)and more readable.
- [direnv](https://formulae.brew.sh/formula/direnv): I don't use this as much as I should, but lets you do fancy stuff like [adjust environment variables based on the current directory](https://direnv.net/).
- [gh](https://formulae.brew.sh/formula/gh): Command-line [tool for GitHub stuff](https://github.com/cli/cli). New, but cool.
- [git-extras](https://formulae.brew.sh/formula/git-extras): Lots of [extra helper stuff](https://github.com/tj/git-extras/blob/master/Commands.md) for `git`
- [hub](https://formulae.brew.sh/formula/hub): Some GitHub [things](https://github.com/github/hub) that `gh` doesn't quite do...yet.
- [mas](https://formulae.brew.sh/formula/mas): CLI for the Mac App Store. If you want to install MAS stuff via `Brewfile`, you need this.
- [ponysay](https://formulae.brew.sh/formula/ponysay): Pipe text through this to have [a cute pony display it](https://github.com/erkin/ponysay). Whimsy!
- [speedtest](https://formulae.brew.sh/formula/speedtest): Official CLI for [speedtest.net](https://speedtest.net). 
- [thefuck](https://formulae.brew.sh/formula/thefuck): Corrects your [previous console command](https://github.com/nvbn/thefuck).
- [tldr](https://formulae.brew.sh/formula/tldr): Replacement for `man`.
- [tree](https://formulae.brew.sh/formula/tree): Why this isn't part of the standard OS X, I will never know.
- [vim](https://formulae.brew.sh/formula/vim): Yes, OS X includes `vim`. But some plugins I like need it compiled with lua support, so there.
- [yadm](https://formulae.brew.sh/formula/yadm): I use this to manage my [dotfiles](https://github.com/mattstratton/matty-dotfiles).
- [youtube-dl](https://formulae.brew.sh/formula/youtube-dl): Command-line tool to download videos from YouTube links.
- [zsh-syntax-highlighting](https://formulae.brew.sh/formula/zsh-syntax-highlighting): A plugin for zsh to make your command line life much easier. 
- [zsh-autosuggestion](https://formulae.brew.sh/formula/zsh-autosuggestion): Another really helpful zsh plugin.

## Casks

Homebrew can also install applications that have installers, etc. I try to only install software using a cask so that I can keep it tracked with my `Brewfile`. Note that some of these applications are not free and will require you to input a license key the first time you start them up. I haven't included *every* cask that I use, because do you really care that I install Docker via cask? No, you don't.

- [1password](https://formulae.brew.sh/cask/1password): This is my main password management application. I personally like it because I can use it across my mobile devices as well as all my computers. Use the one you prefer, of course, but you should be using one!
- [adobe-creative-cloud](https://formulae.brew.sh/cask/adobe-creative-cloud): This gets the main application installer/control on my machine so that I can install the various Adobe applications that I am licensed to use. 
- [aerial](https://formulae.brew.sh/cask/aerial): An OS X screensaver that uses the same images/look as the Apple TV screensaver. 
- [airfoil](https://formulae.brew.sh/cask/airfoil): A great product from Rogue Amoeba to redirect output to various Airplay devices. I use this to stream Spotify to my HomePod.
- [audio-hijack](https://formulae.brew.sh/cask/audio-hijack): Rogue Amoeba again! Dump audio from any application to be recorded, etc.
- [authy](https://formulae.brew.sh/cask/authy): As much as possible, I use Authy for my OTP/multi-factor authentication. I can use it on my phone, as well as keep them in sync across all my devices. This means I don't need to create a new code for Google, etc when I get a new phone!
- [alfred](https://formulae.brew.sh/cask/alfred): Task launcher (and more). I'll eventually write up a post detailing the various Alfred workflows that make my life easier. Replaces Spotlight for launching apps by search, and also includes a great clipboard replacement.
- [bartender](https://formulae.brew.sh/cask/bartender): Small utility that you don't know you needed until you try it. Lets you hide various things in the Mac menubar. Awesome.
- [beyond-compare](https://formulae.brew.sh/cask/beyond-compare): I use this for diffing files. Maybe it's a force of habit, maybe you have a better tool you like. YMMV.
- [cakebrew](https://formulae.brew.sh/cask/cakebrew): A GUI in front of Homebrew. Necessary? No. Kind of neat? Yes.
- [dash](https://formulae.brew.sh/cask/dash): Great tool for quick access to documentation on various tools, languages, etc. Coupled with Alfred, it's amazing.
- [dropbox](https://formulae.brew.sh/cask/dropbox): I go back and forth with Dropbox; I keep my documents in iCloud, but Dropbox is great for syncing certain files (for example, I keep my Alfred settings in sync via Dropbox) and also, this is where I keep images, movie files, etc.
- [elgato-control-center](https://formulae.brew.sh/cask/elgato-control-center): Tool for controlling my [Elgato Key Lights](https://www.amazon.com/Elgato-Key-Light-Professional-App-Enabled/dp/B07L755X9G/).
- [obs](https://formulae.brew.sh/cask/obs): If you use the Elgato Stream Deck, note that OBS must be installed before the Stream Deck software. Which annoyed me, because I like my `Brewfile` to be alphabetical.
- [elgato-stream-deck](https://formulae.brew.sh/cask/elgato-stream-deck): This is the driver/configuration utility for the [Stream Deck](https://www.amazon.com/Elgato-Stream-Deck-XL-customizable/dp/B07RL8H55Z), which gives me quick buttons for doing fancy things like controlling the aforementioned Key Lights, as well as shortcuts for cool things in OBS.
- [farrago](https://formulae.brew.sh/cask/farrago): A soundboard for sound effects, etc. 
- [handbrake](https://formulae.brew.sh/cask/handbrake): While I don't rip DVDs anymore, this is still a super useful tool for converting video files to the format I want.
- [iterm2](https://formulae.brew.sh/cask/iterm2): If you do anything in the terminal on OS X, you should be using iTerm. Period.
- [loopback](https://formulae.brew.sh/cask/loopback): Creates virtual audio devices, so it's a helpful audio router.
- [krisp](https://formulae.brew.sh/cask/krisp): Noise cancellation, in case you are taking a Zoom call in a noisy area.
- [logitech-presentation](https://formulae.brew.sh/cask/logitech-presentation) - I mention this one because it's kind of annoying; this only installs the *installer* for the Logitech Spotlight remote; you will then need to run the installer from where it gets dumped at a location like this: `/usr/local/Caskroom/logitech-presentation/1.54.84/LogiPresentation Installer.app`
- [macdown](https://formulae.brew.sh/cask/macdown): My favorite Markdown editor.
- [moom](https://formulae.brew.sh/cask/moom): Window management tool. I use this a lot. I have custom configurations for the placement of windows on the screen, and Moom lets me move windows there with a keystroke. Love it.
- [soundsource](https://formulae.brew.sh/cask/soundsource): Lets me control audio on a per-app basis, adjusting the volume and output device for individual apps, etc.
- [tower](https://formulae.brew.sh/cask/tower): Most of the time, I use `git` at the command line, but this is a nice GUI on top of it.
- [witch](https://formulae.brew.sh/cask/witch): Enhance task switcher, making it easier to tab between windows, etc, not just apps.

## Fonts

You can even use Homebrew to install fonts! I don't have all my fonts in my `Brewfile` because there isn't a cask for every one I use, but I do have these:

```
tap "homebrew/cask-fonts"
cask "font-hack-nerd-font"
cask "font-inconsolata-for-powerline"
cask "font-menlo-for-powerline"
```

Notice that I need to add a tap in order to get those fonts.

## Mac App Store apps

I am not going to list all these, as I only use a few (mostly games), but just to touch on a few things.

You need to know the ID of the app; to get it, run the following command:
`mas search Bear` (where "Bear" is the search string for the app you want). You need the `mas` package installed for this, which is why we have the packages listed first in the `Brewfile`.

You'll get output that looks like this:

```
  1091189122  Bear                             (1.7.11)
   926066161  Wildlife Simulator: Bear         (1.0)
   413013033  BATTLE BEARS -1 Mac              (1.1)
  1150538527  Dress Up Bear                    (1.1)
   792252100  Build A Teddy Bear               (1.0)
   418326655  Beargo                           (1.3)
   675102891  Teddy Bear : Kindergarten        (1.0)
   639585198  Little Bear: My very first games (1,00)
   612122909  Berenstain Bears Get In a Fight  (1.2)
   612126526  Berenstain Bears In the Dark     (1.2)
   
```
The first column is the ID that you will need. You also need the *exact* app name in the second column. Then, update your `Brewfile` like this!

```
mas "Bear", id: 1091189122
```
It's that easy!
