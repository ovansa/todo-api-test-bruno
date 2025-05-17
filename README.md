# 🧪 todo-api-test-bruno

API tests for a Todo application using [Bruno](https://www.usebruno.com/), a Git-friendly and open-source API client. It includes tests for authentication and Todo CRUD operations, and supports both local and CI testing workflows.

## 📁 Project Structure

```
todo-api-test-bruno/
├── Auth/                     # Authentication test requests
├── Todo/                     # Todo CRUD test requests
├── environments/             # Environment configurations
├── .github/workflows/test.yml # GitHub Actions workflow
├── collection.bru            # Bruno collection
├── bruno.json                # Bruno config
└── package.json              # Project metadata
```

## 🚀 Getting Started

### Prerequisites

* [Bruno](https://www.usebruno.com/)
* Node.js
* (Optional) [naktos](https://github.com/naktos/naktos) for running GitHub Actions locally

### Installation

```bash
git clone https://github.com/ovansa/todo-api-test-bruno.git
cd todo-api-test-bruno
npm install
```

## 🧪 Running Tests

### Using Bruno GUI

1. Open Bruno and load the `collection.bru` file.
2. Set the environment variables.
3. Run requests and review the tests.

### Using Bruno CLI

```bash
npm install -g @usebruno/cli
bruno run collection.bru
```

### Running GitHub Actions Locally

This project includes a GitHub Actions workflow (`.github/workflows/test.yml`) to automate API test runs. You can run this workflow locally using [naktos](https://github.com/naktos/naktos):

```bash
naktos run .github/workflows/test.yml
```

## ⚙️ Environment Variables

Environment configurations are located in the `environments/` directory. Set these correctly before running tests.


## 🛠 Related Projects

* [Todo API (Go)](https://github.com/ovansa/todo-app-go) — The backend this suite tests.
