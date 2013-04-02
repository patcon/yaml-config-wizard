yaml-config-wizard
==================

A placeholder for a gem that will allow for the easy creation of an interactive YAML config from a template.

Requirements
------------

- point the gem to yaml template, and when command is run, prompt for each value, showing default like so:

        $ commandname
        >> domain? <defaultdomain.com> mycustomdomain.com
        >> second_key? <secondvalue> override second value
        
  The above will save a yaml file to a pre-defined location (different from template).
- Running the command again will show the default as the current yaml directive's values, but will allow them to be changed.
- When the value is an array, implode it into a comma-separated string, then explode it back out when building YAML.
- How can we provide more dynamic prompting without sacrificing simplicity of template approach? Read comments in template?
- variables:
  - template_path
  - config_path
