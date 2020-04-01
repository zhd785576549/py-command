# py-command

A simple command tool

### Install

```shell script
git clone https://github.com/zhd785576549/py-command
cd py-command
python setup.py install
```

### Sample

```python
from py_command.entry import CommandManager
import os


if __name__ == '__main__':
    sub_command_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "subcommand")
    command_manager = CommandManager(sub_command_module_path="test.subcommand", sub_command_path=sub_command_path)
    command_manager.execute_from_argv()
```
