## Best VSCode Settings

Especially for *Python*, *Django* and *JavaScript* :heart:

---

### Setup

If you are using Arch Linux:

```sh
# for Python/Django
sudo pacman -S python-pylint autopep8 --noconfirm
yay -S python-pylint-django --noconfirm
```

```sh
# and for JS
sudo pacman -S eslint --noconfirm
```

```sh
# my prefered font (extra)
sudo pacman -S otf-fira-code
```

---

### Extensions

List of extensions that you need:
- Python
- Prettier
- and done!

---

### Settings

Now, just copy and paste the settings:

```json
{
  "editor.fontLigatures": true,
  "editor.fontFamily": "'Fira Code', monospace",

  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  "[javascript]": {
    "editor.formatOnSave": true
  },

  "[python]": {
    "editor.tabSize": 4,
    "editor.formatOnSave": true
  },
  "python.formatting.autopep8Path": "/usr/bin/autopep8",

  "python.linting.pylintPath": "/usr/bin/pylint",
  "python.linting.pylintArgs": ["--load-plugins", "pylint_django"],
  
  "python.sortImports.path": "/usr/bin/isort"
}
```
