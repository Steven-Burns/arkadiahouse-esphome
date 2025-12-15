arkadiahouse-esphome holds the source code for building esphome-based binary images for the gadgets used in the home automation system of Arkadia House.

!include paths in the source files contained in this repo are absolute paths.
That's because esphome's !include YAML extension does not support parameterizing or using substitutions with the !include file path -- so one cannot parameterize paths.

So, this means that the repo needs to be mounted:
1) On a named volume (for performance on Windows/Mac hosts)
2) At a mount point named /workspace

... which is how the .devcontainer/devcontainer.json is configured.



