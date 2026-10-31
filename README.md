![Banner](banner.png)

# harden-chs-RollbackScriptGenerator
Generates a rollback script from a given configuration hardening script, allowing administrators to easily revert changes if necessary. Uses the 'before' state of any configuration change to construct the rollback. Requires changes in the original script to add 'before' state logging. - Focused on Extracts the '#BEFORE:' records logged in a hardening script (including indented records) and writes those commands, in reverse order, into an executable rollback script. That extraction is all the tool does: no policy files are parsed, no templates are rendered, and no hardened configuration is built. A run exits 1 when the input is missing, when no '#BEFORE:' commands are extracted, when the rollback script cannot be written, or when the rollback path resolves to the hardening script itself, in which case the input is left untouched.

## Install
`git clone https://github.com/ShadowStrikeHQ/harden-chs-rollbackscriptgenerator`

## Usage
`./harden-chs-rollbackscriptgenerator [params]`

## Parameters
- `-h`: Show help message and exit
- `--dry-run`: Perform a dry run without writing the rollback script.

## License
Copyright (c) ShadowStrikeHQ
