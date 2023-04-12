# Copilot PR First Comment Updater

The `copilot-pr-first-comment-updater` is a Python script that appends the `copilot:all` label to the first comments of closed pull requests in a specified GitHub repository, allowing easy tracking and management of processed PRs.

## Prerequisites

- Python 3.6 or higher
- A GitHub personal access token with the necessary permissions (e.g., `repo` scope)

## Installation

1. Clone this repository:

`git clone https://github.com/yigitkonur/copilot-pr-first-comment-updater`


2. Change the directory to the cloned repository:

`cd copilot-pr-first-comment-updater`

3. Install the required dependencies:

`pip install PyGithub`


## Configuration

Open the `update_prs.py` script with your favorite text editor and replace the following variables with your own values:

- `ACCESS_TOKEN`: Replace with your GitHub personal access token.
- `REPO_NAME`: Replace with the target repository in the format `your_username/repo_name`.

## Usage

Run the script by executing the following command:

`python3 update_prs.py`

The script will process all closed pull requests in the specified repository and append the `copilot:all` label to the first comment. It will skip PRs that have already been processed or contain a 'Generated by Copilot' label.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
