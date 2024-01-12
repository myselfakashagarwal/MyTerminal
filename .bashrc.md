# Environment setup 

The .bashrc is executed every time a user logins, if not in your case you can do this `echo "source .bashrc" >> .bash_profile`. This is specific to bash if you are using zsh shell you can modify script accordingly. 

For bash setup remove stuff accordingly and paste all the stuff in your .bashrc file in your home directory; make sure to restart the terminal again to see changes (not tabs)

```bash

# Exporting colours; they can be accessed across all child sessions 
export BROWN='\033[38;5;94m'
export ORANGE='\033[38;5;208m'
export GREEN='\[\e[32m\]'
export YELLOW='\033[1;33m'
export RED='\033[0;31m'
export BLUE='\033[0;34m'
export PURPLE='\033[0;35m'
export NOCOLOR='\[\e[0m\]'
export PINK='\033[0;95m'
export CYAN='\033[0;36m'
PROMPT='\e[K  \n −−▶︎ '

# The below block of code detects git repo if detected it will create a bundle of information
# In case a git repo is not detected it does not change anything 
# Moving from git repo to normal directories will be auto updated 

export PS1="${GREEN} \u ${PURPLE} \h ${BROWN} \w ${PROMPT}"

get_git_info() {
    local branch head
    if branch=$(git branch -v 2>/dev/null | grep "^*" | awk '{ print $2 }'); then
        head=$(git branch -v 2>/dev/null | grep "^*" | awk '{ print $3 }')
        status=$(git status -v 2>/dev/null | awk 'NR==4 { print }')
        echo "${PURPLE} ${branch} ${BLUE} ${head} ${YELLOW} ${status} ${NOCOLOR} "
    else
        echo ""
    fi
}

# Update prompt will update PS1 variable with the bundle of information provided by get_git_info
# More functions can also be added aprt from git; init just attach the output of new function to PS1 

update_prompt() {
    local git_info
    git_info=$(get_git_info)
    if [ -n "$git_info" ]; then
        PS1="${GREEN} \u ${PURPLE} \h ${BROWN} \w ${git_info} ${PROMPT}"
    else
        PS1="${GREEN} \u ${PURPLE} \h ${BROWN} \w ${PROMPT}"
    fi
}

# Prompt command is a environment variable it holds the command that is to be executed before each prompt 

PROMPT_COMMAND=update_prompt
clear


# Clear command for rehl 
# For rhel based distros clear command is not present by default; becasue it a GNU's command from realine library
# You can mimic the behaviour of clear using ANSI codes 
alias clear="echo -e '\033[H\033[2J\033[3]'"
export clear
# In case you want to use it as a command just create a file named clear in /usr/local/bin 
# in that file write → clear="echo -e '\033[H\033[2J\033[3]'"              you are all done 
# Do not use this in case you have a clear command preinstalled (it will create a blackhole)


# Get IPv4
alias myip=curl -4 -s https://ipv4.icanhazip.com
export myip

```

They are most used for me drop yours if you have some 