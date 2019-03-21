# Godot TODO Tracker Plugin

Easily keep track of items on your 'todo' list directly in the editor!

## Features

- Ability to add, edit, and delete items
- Saves to configurable location
- Saves as INI file
- Automatic backups of todo list
- Scans source files and adds items to list

## Source File Scanning

The plugin can be set up to scan all gdscript files in a user specified location.

For an item to be automatically added they must look like the following in the source:

```
# TODO work on better scanning logic
#  although what we have now is decent enough, it 
#  could be a lot faster and more memory efficient
```

The text next to the `TODO` statement will be picked up and saved as the todo item title and every
comment underneath will be saved along as the comment.