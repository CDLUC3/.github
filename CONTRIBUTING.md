# Contributing Guidelines Template

Thank you for your interest in contributing! 🎉  

We welcome all contributions — from bug fixes and documentation improvements to major feature implementations.  
Please take a few minutes to review this guide before submitting your contribution.

This guide provides general information to supplement the official contribution documentation. For detailed processes, policies, and best practices, please refer to a project/repositories CONTRIBUTING.md file.
## How to Report Issues
- Use [GitHub Issues] for bugs and feature requests.
- Include as much detail as possible.

## Code of Conduct
Please review and follow our [Code of Conduct](CODE_OF_CONDUCT.md).

## License
By contributing, you agree that your contributions are licensed under the [MIT License](LICENSE.md).

---

## 🧭 How to Contribute

### 1. Fork the Repository
Start by forking this repository to your own GitHub account:

```bash
git clone <repository_name>
cd <repository_name>
```

### 2. Create a Branch
Create a new branch for your feature or bug fix.
```bash
git checkout -b feature/your-feature-name
```

Please use the following naming convention:
- `feature/your-feature-name` for new features
- `bug/your-bug-description` for bug fixes
- `docs/your-documentation-update` for documentation changes (e.g. README, comments)
- `chore/your-chore-description` for maintenance tasks (e.g. updating dependencies)

### 3. Make Your Changes
Make your changes in your local repository. Please ensure that your code adheres to the project's coding standards and conventions.

For information on how to set up your development environment, please refer to the [README.md](README.md).

Use a linter.

Recommended: Use a `CHANGELOG.md` file to document all notable changes made to the project. Please update this file with a brief description of your changes, following the existing format.

### 4. Test Your Changes
Please write unit tests for your changes and ensure all tests pass before submitting!

### 5. Commit Your Changes
Commit your changes with a clear and concise commit message with what you've done.
```bash
git add .
git commit -m "Add your commit message here"
```

Please ensure that your code passes any prehook/precommit checks.

### 6. Make sure your branch is up to date
Before pushing your changes, make sure your branch is up to date with the main branch. From your branch run:
```bash
git pull origin main
```

### 7. Push Your Changes
Push your changes to your forked repository:
```bash
git push origin feature/your-feature-name
```

### 8. Create a Pull Request
Go to the original repository and create a pull request from your forked repository. Follow the template provided and include as much detail as possible including instructions for how to test the change if applicable.
Be sure to reference the issue number if your pull request addresses a specific issue!

### 9. Address Feedback
We may request changes or provide feedback on your pull request. Please address any feedback promptly to help us review and merge your changes.

We are a small team and may not be able to respond immediately, but we will do our best to review your contribution as soon as possible.

### 10. Celebrate!
Once your pull request is merged, celebrate your contribution to the project! 🎉
