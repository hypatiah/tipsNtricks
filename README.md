# Tip && Tricks
## For the JR Dev in your life.
**Literally** every thing below is IMHO




### Pro Tip Numero Uno

__HANDS OFF THE F*&^%ING MOUSE!!!__

As a developer your time is a __Super Valuable Resource__...

So every little thing you can do to increase efficiency will pay vast dividends over the course of your career.

You rarely need to actually touch the mouse. Every time you do you must take your hands complete off the keyboard. Grab the mouse. Go click the thing, then transfer back to the keyboard, find the home-row and finally start typing again...Precious seconds that add up to a huge savings.

Turns out ```⌘ p``` is the fastest way to get around a working directory.

### Take care of yourself

This job can be very grueling. Your personal sanity is a thing you should be mindful of always.
  - Eat well
  - Exercise often
  - Yoga is great
  - Work life balance (**after dbc**) is super important
  - Always remember __You are not your Code__

### Follow the Golden Rule of BLOCKS
As soon as you __OPEN__ the block __CLOSE__ the block.
```ruby

def thing_func

end

thingy.each do

end

{ }

[ ]

```

### Code readability BEATS conciseness 10.times out of 10
This means writing functions that are easy for developers to read. Not just you, but the people that maintain your code down the road.

Don't one line a thing because you want to look cool.
Indentation - OMG do this. All the time. No matter what. Lots of languages are whitespace dependent, meaning you must indent correctly. Better to establish this habit now.

![MaintainYourShit](./readability.jpeg "Fer Realsies")

## Chrome Extensions
[Recomendations](https://github.com/bootcoder/htc_dev_settings/blob/master/chrome_extensions.md)

## Hot Key your iTerm2
```⌘+\``` is what I use.

Also.... Use iTerm2 instead of terminal.

## Sublime Packages
  * Package Manager
  * Better CoffeeScript
  * BracketHighlighter
  * ERB Snippets
  * GitGutter
  * Haml
  * JSLint
  * Markdown HTML Preview
  * Package Control
  * PowerCursors
  * SideBarEnhancements
  * sublime-github
  * SublimeLinter
  * SublimeLinter-haml
  * TernJS
  * Theme - Brogrammer
  * Tomorrow Color Scheme

## Sublime Shortcuts
[Complete List](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/reference/keyboard_shortcuts_osx.html)

Super useful ones
- move lines vertically
- jump to line
- jump to file
- global search
- duplicate line
- select word (and repeat)

### Linters
The good the bad and the ugly
Pros
  - help you see errors in your code
  - give you tips on best practices
  - easy to use

Cons
  - can cause stability issues with Sublime
  - others best practices may not always align with your own.


## NO SUDO NO(osx only)

## BASH Aliases
```bash
alias e=subl
alias be="bundle exec"
alias g=git
alias cl=clear
alias ga="git ca"
alias gpo="git push origin"
alias gph="git push heroku"
alias db:reset="be rake db:drop && be rake db:create && be rake db:migrate && be rake db:test:prepare && be rake db:seed && rails c"
alias rials="rails"
alias gti="git"
alias shitgun="shotgun"
alias shotfun="shotgun"
alias dbc="cd ~/Dropbox/ACODE/DBC/dayJerbs"
alias code="cd ~/Dropbox/ACODE/adBC
```

## GIT Config
```bash
[core]
  # Excludesfiles allows us to set a global list of things to ignore
  excludesfile = ~/.gitignore_global

# These are custom color options for the console
[color]
  status = auto
  diff = auto

[color "status"]
  untracked = cyan
  changed = green
  added = yellow

# Aliases are command shortcuts
[alias]

  # lg is now a shortcut for a pretty log with short commit messages
  # See the log manpage: https://www.kernel.org/pub/software/scm/git/docs/git-log.html
  # for explanations of what these options do

  lg = log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative

  # Shorthand for a less noisy status
  s = commit --dry-run --short

  # More sensible names for adding and removing files from the readme
  stage = add
  unstage = reset HEAD

  # Edit the last commit
  amend= commit --verbose --amend

  # one-line log
  l = log --pretty=format:"%C(yellow)%h\\ %ad%Cred%d\\ %Creset%s%Cblue\\ [%cn]" --decorate --date=short

  a = add
  ap = add -p
  c = commit --verbose
  ca = commit -a --verbose
  cm = commit -m
  cam = commit -a -m
  m = commit --amend --verbose

  d = diff
  ds = diff --stat
  dc = diff --cached

  co = checkout
  cob = checkout -b

  # list branches sorted by last modified
  b = "!git for-each-ref --sort='-authordate' --format='%(authordate)%09%(objectname:short)%09%(refname)' refs/heads | sed -e 's-refs/heads/--'"

  # list aliases
  la = "!git config -l | grep alias"
[user]
  email = bootcoder@gmail.com
  name = BootCoder
[credential]
  helper = cache --timeout=14400

```

## APPS (osx)
  - Flycut (clipboard management)
  - Spectacle (window management)
  - Dropbox
  - Alfred
  - Dash
  - PostMan REST Client

## Links
[Tips for JR Devs](https://blog.newrelic.com/2014/04/23/better-junior-developer/)
[10 Tips to transition from JR to MID level Dev](http://www.techrepublic.com/blog/software-engineer/10-tips-to-go-from-a-beginner-to-an-intermediate-developer/)



## BASH TIPS
control + r == reverse search
history
man + / for search
fn + leftArrow || fn + rightArrow key for front or end of line
