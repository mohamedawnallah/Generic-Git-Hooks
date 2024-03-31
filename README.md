# Generic Git Hooks

These Git hooks are designed to streamline the contribution process by enforcing various guidelines commonly found across open-source projects. By integrating these hooks into your workflow, you can ensure consistency and adherence to contribution standards, saving time and effort in the development process.

## Features

- **Commit-msg Hooks**: Enforce commit message conventions to maintain a clean and informative commit history.
- **Post-checkout Hooks**: Trigger actions after a checkout has been completed, such as updating dependencies or resetting project state.
- **Post-commit Hooks**: Execute tasks automatically after a commit has been made, such as generating documentation or running tests.

## Installation

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/mohamedawnallah/generic-git-hooks.git
    ```

2. Navigate to the cloned repository directory:

    ```bash
    cd generic-git-hooks
    ```

3. Copy the hooks you wish to use to your project's `.git/hooks` directory:

    ```bash
    cp hooks/commit-msg /path/to/your/project/.git/hooks/
    cp hooks/post-checkout /path/to/your/project/.git/hooks/
    cp hooks/post-commit /path/to/your/project/.git/hooks/
    ```

4. Make the hooks executable:

    ```bash
    chmod +x /path/to/your/project/.git/hooks/commit-msg
    chmod +x /path/to/your/project/.git/hooks/post-checkout
    chmod +x /path/to/your/project/.git/hooks/post-commit
    ```

## Usage

Once installed, the hooks will automatically execute at their respective stages in the Git workflow. Any violations or issues detected by the hooks will prevent the corresponding action (commit or push) from proceeding until resolved.

To customize the behavior of the hooks, you can edit the scripts directly or modify them to suit your project's specific requirements.

## Contributing

Contributions are welcome! If you have suggestions, improvements, or additional hooks to share, please feel free to open an issue or pull request on GitHub.

## License

This project is licensed under the [MIT License](LICENSE).

