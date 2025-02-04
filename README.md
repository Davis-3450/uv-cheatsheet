# UV Command Cheat Sheet (Sorted by Relevance) 🚀

UV is a blazing‑fast Python package and project manager written in Rust. It "replaces" tools like pip, pip‑tools, pipx, poetry, pyenv, twine, virtualenv, and more. Here’s a quick reference guide to help you navigate uv.

---

## Most Common Commands ✨

**uv init**  
Initializes a new project and creates the basic files (e.g. pyproject.toml).  
```bash
uv init myproject
```

**uv add**  
Adds a dependency to your project (updates pyproject.toml, lockfile, and environment).  
```bash
uv add django
```

**uv sync**  
Synchronizes your project environment by installing or updating dependencies.  
```bash
uv sync
```

**uv run**  
Runs a command or script in your project environment. It auto‑syncs before execution.  
```bash
uv run manage.py runserver
```

**uv pip**  
A pip‑compatible interface for installing packages or compiling dependency files.  
```bash
uv pip install requests  
uv pip compile requirements.in -o requirements.txt
```

---

## Python Version & Environment Management 🐍

**uv python**  
Manages Python versions. Use it to install new versions or pin your project’s Python.  
```bash
uv python install 3.12  
uv python pin 3.11
```

**uv remove**  
Removes a dependency from your project.  
```bash
uv remove django
```

---

## Extended Workflow Commands 🔍

**uv tool**  
Manages CLI tools (like pipx). Run, install, list, upgrade, or uninstall tools.  
```bash
uv tool run ruff  
uv tool install ruff
```

**uv lock**  
Updates your project’s lockfile without syncing the environment.  
```bash
uv lock --upgrade
```

**uv tree**  
Displays your dependency tree so you can quickly see package relationships.  
```bash
uv tree
```

**uv export**  
Exports your lockfile (e.g. to a requirements.txt file).  
```bash
uv export --output-file requirements.txt
```

---

## Less-Frequent (But Important) Commands 🔧

**uv build**  
Builds your project’s distributions (source or wheel).  
```bash
uv build
```

**uv publish**  
Publishes your package to an index (like PyPI).  
```bash
uv publish
```

**uv cache**  
Manages uv’s cache (clean, view cache directory, etc.).  
```bash
uv cache clean  
uv cache dir
```

**uv self update**  
Updates uv itself to the latest version.  
```bash
uv self update
```

**uv version**  
Displays the current uv version.  
```bash
uv version
```

**uv generate-shell-completion**  
Generates shell completion scripts for your terminal.  
```bash
uv generate-shell-completion bash > ~/.bash_completion
```

**uv help**  
Shows help information for all available commands.  
```bash
uv help
```

---

## Final Recap ✅

Sorted by relevance, here’s the list:

- uv init
- uv add
- uv sync
- uv run
- uv pip
- uv python
- uv remove
- uv tool (and subcommands)
- uv lock
- uv tree
- uv export
- uv build
- uv publish
- uv cache
- uv self update
- uv version
- uv generate-shell-completion
- uv help

This cheat sheet is sorted by how common the commands are in everyday workflows. Enjoy the simplicity and speed uv brings to your Python projects! Happy coding! 😄👍
