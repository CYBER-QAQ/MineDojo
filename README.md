## Modified MineDojo Package

### Installation

Uninstall your minedojo package.

Clone this repo. Run `python setup.py install`

### Modification

- In `minedojo/tasks/__init__.py`: 

Function `__specific_task_make`. Deep copy task_specs, to support repeatedly making one environment in a program. Remove keys in task_specs that appear in kwargs, to enable modifying the default args predefined by programmatic tasks when calling env.make().

- In `minedojo/sim/Malmo/Minecraft/build.gradle`, and `minedojo/sim/Malmo/Minecraft/gradle/wrapper/gradle-wrapper.properties`:

Use the mirror urls.
