# Project File Tree (prft)

prft is a Python library designed to easily generate and display the file structure of a project, with support for .gitignore patterns. It allows you to quickly visualize the organization of files and directories within a specified project directory.

## Features
-	Generates a clear and visual representation of your project’s file structure.
-	Supports .gitignore and other ignore files, so you only see files relevant to the project.
-	Allows hiding hidden files (dotfiles) for a cleaner output.
-   Easy to use for ChatGPT.

## Installation
Install prft via pip:
```bash
pip install prft
```

## Usage
Use prft in the terminal to display a project’s file structure.

**Basic Command**
```bash
prft path_to_project
```

You can also use . to specify the current directory if you are in the project directory:

```bash
prft .
```

### Options
- **--no-ignore**: Show all files, including those listed in .gitignore.
- **--no-dot**: Include hidden files (dotfiles) in the output.
- **--prefix** "some prefix": Use your own prefix (" " by default)

**Example:**
```bash
prft path_to_project --no-ignore --no-dot
```

### Example Output

Running prft in a sample project directory might produce output like this:
```
project/
├── src/
│   ├── main.py
│   ├── utils.py
│   └── config/
│       └── settings.py
├── .gitignore
├── README.md
└── requirements.txt
```
This output shows a hierarchical view of the files and directories in *path_to_project*, ignoring files specified in .gitignore (unless `--no-ignore` is used).

## License

This project is licensed under the MIT License.

## Author

Created by [trum-ok](https://github.com/Trum-ok) :p
