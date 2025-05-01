# harden-chs-RollbackScriptGenerator
Generates a rollback script from a given configuration hardening script, allowing administrators to easily revert changes if necessary. Uses the 'before' state of any configuration change to construct the rollback. Requires changes in the original script to add 'before' state logging. - Focused on Generates hardened configuration files (e.g., SSH, web servers, databases) based on predefined security policies and user-defined parameters.  Leverages YAML for policy definitions and Jinja2 for templating, allowing for customized hardening scripts tailored to specific environments and compliance requirements.  Focuses on automating the creation of secure-by-default configurations.

## Install
`git clone https://github.com/ShadowStrikeHQ/harden-chs-rollbackscriptgenerator`

## Usage
`./harden-chs-rollbackscriptgenerator [params]`

## Parameters
- `-h`: Show help message and exit
- `--dry-run`: Perform a dry run without writing the rollback script.

## License
Copyright (c) ShadowStrikeHQ
