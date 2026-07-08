# GitHub-Access-Auditor
A Bash automation tool that uses the GitHub REST API to list repository collaborators with read access using cURL and jq.


# GitHub Access Auditor

A simple Bash-based automation tool that uses the GitHub REST API to list repository collaborators with read access. This project demonstrates API integration, Bash scripting, authentication using GitHub Personal Access Tokens, and JSON parsing with `jq`.

## Features

* Lists repository collaborators
* Identifies users with read (pull) access
* Uses the GitHub REST API
* Authenticates using a GitHub Personal Access Token (PAT)
* Parses JSON responses using `jq`
* Lightweight and easy to extend

## Tech Stack

* Bash
* GitHub REST API
* cURL
* jq

## Prerequisites

Before running the script, ensure you have:

* Bash
* cURL
* jq
* A GitHub Personal Access Token with the required repository permissions

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/github-access-auditor.git
cd github-access-auditor
```

Install `jq` if it is not already installed.

Ubuntu/Debian:

```bash
sudo apt install jq
```

macOS:

```bash
brew install jq
```

## Configuration

Export your GitHub credentials as environment variables:

```bash
export username="your_github_username"
export token="your_personal_access_token"
```

## Usage

Run the script by providing the repository owner and repository name:

```bash
./script.sh <repository_owner> <repository_name>
```

Example:

```bash
./script.sh octocat Hello-World
```

## Sample Output

```text
Listing users with read access to octocat/Hello-World...

Users with read access to octocat/Hello-World:

user1
user2
user3
```

## Project Structure

```text
github-access-auditor/
│
├── script.sh
├── README.md
└── LICENSE (optional)
```

## Skills Demonstrated

* Bash scripting
* Shell functions
* REST API integration
* GitHub API authentication
* Environment variables
* JSON parsing using jq
* Linux command-line automation

## Future Improvements

* Display collaborator permission levels (Read, Write, Admin)
* Export reports to CSV or JSON
* Generate HTML reports
* Send email notifications
* Integrate with GitHub Actions
* Add repository security checks
* Audit multiple repositories in a single run

## License

This project is available under the MIT License.
