![GitHub repo size](https://img.shields.io/github/repo-size/GitKinetic/my-configs)
![License](https://img.shields.io/github/license/GitKinetic/my-configs)

# My Configurations

This repository contains my personal configuration files for Git, shell, and IDEs. These configurations are designed to streamline developer workflows, enhance productivity, and maintain privacy. Feel free to explore, use, or adapt them as needed.

## Files Included

### Git Configurations (`git/.gitconfig`)
- **Purpose**: Simplifies Git commands and ensures privacy with GitHub's noreply email.
- **Features**:
  - Aliases:
    - `co` → `git checkout`
    - `cm` → `git commit`
    - `st` → `git status`
    - `lg` → `git log --oneline --graph --decorate`
  - Privacy settings to hide your personal email in commits.

### Shell Configurations (`shell/.bashrc`)
- **Purpose**: Enhances command-line efficiency with custom aliases and environment variables.
- **Features**:
  - Aliases:
    - `ll` → `ls -la`
    - `gs` → `git status`
    - `gc` → `git commit`
  - Adds frequently used paths to the `$PATH` variable.

### VS Code Settings (`ide/settings.json`)
- **Purpose**: Provides a consistent and optimized development environment in VS Code.
- **Features**:
  - Auto-formatting on save.
  - Preferred extensions:
    - Prettier for code formatting.
    - GitLens for advanced Git features.
  - Custom keybindings for productivity.

---

## Usage

### Step 1: Clone the Repository
```bash
git clone https://github.com/GitKinetic/my-configs.git
```
### Step 2: Apply the Configurations

- **Git**:
  - To use the custom `.gitconfig` file, copy it to your home directory and include it in your global Git configuration:
    ```bash
    cp git/.gitconfig ~/.gitconfig
    git config --global include.path ~/.gitconfig
    ```

- **Shell**:
  - To use the `.bashrc` file, copy it to your home directory and source it:
    ```bash
    cp shell/.bashrc ~/.bashrc
    source ~/.bashrc
    ```

- **VS Code**:
  - To apply the `settings.json` file, copy it to your VS Code user settings directory:
    ```bash
    mkdir -p ~/.config/Code/User
    cp ide/settings.json ~/.config/Code/User/settings.json
    ```


## License
This repository is licensed under the MIT License. You are free to use, modify, and distribute these configurations. See the full license [here](LICENSE).


## Contributing
Contributions are welcome! If you have suggestions or improvements, feel free to fork the repository and open a pull request.

To contribute:
1. Fork the repository.
2. Create a new branch for your changes (`git checkout -b feature-branch`).
3. Commit your changes with clear messages.
4. Open a pull request for review.

