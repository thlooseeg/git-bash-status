

# Git-Bash-Status

Enhance bash prompt to include git repo information

## Features

The prompt will show 

1. Repo name (will use remote origin if available)
2. Current branch name
3. Status (via colors & symbols)

in the following format:

    $color$repo_name ($branch_name) $indicator

The repo status will be displayed as follows:

* Uncommitted Changes (dirty working directory) - red text with indicator "*"
* Ahead of Origin - Yellow text with indicator "✘"
* Up to date - Green text with indicator "✓"

**The configuration also defines PS1 as follows:**

Inside Git repo:

    "$WHITEBOLD[$BLACKBOLD\u $WHITEBOLD\A $PURPLE\w$WHITEBOLD $(git-info) $WHITEBOLD] $ $NO_COLOUR"

Not in Git repo:

    "$WHITEBOLD[$BLACKBOLD\u $WHITEBOLD\A $PURPLE\w$WHITEBOLD] $WHITEBOLD$ $NO_COLOUR"

The path information is shortend to include only the last two components.

## Setup

Source the script in your .bashrc like this

```
source /path/to/bash-git-status
```

## License

  [Public Domain](LICENSE)

## Thanks to

This is a modified version of 

  [orourkek/Bash-Git-Status](https://github.com/orourkek/Bash-Git-Status)

