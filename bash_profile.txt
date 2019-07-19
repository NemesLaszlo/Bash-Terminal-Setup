# Enable tab completion
source ~/git-completion.bash

# colors!
green="\[\033[0;32m\]"
blue="\[\033[0;34m\]"
purple="\[\033[0;35m\]"
reset="\[\033[0m\]"
yellow="\[\033[0;33m\]"
Red="\[\033[0;31m\]"
UCyan="\[\033[4;36m\]"
Cyan="\[\033[0;36m\]"
On_Yellow="\[\033[43m\]"

# Change command prompt
source ~/git-prompt.sh
export GIT_PS1_SHOWDIRTYSTATE=1
# '\u' adds the name of the current user to the prompt
# '\$(__git_ps1)' adds git-related stuff
# '\W' adds the name of the current directory
export PS1="$Cyan \A $yellow\u$Red \w $ $green\$(__git_ps1) $reset"

#colorize the terminal output
alias ls='ls -G'
alias ll='ls -lG'

# Tell ls to be colourful
export CLICOLOR=1
export LSCOLORS=exfxcxdxbxegedabagacad

# Tell grep to highlight matches
export GREP_OPTIONS='--color=auto'
