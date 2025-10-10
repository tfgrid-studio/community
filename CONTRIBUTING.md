# Contributing to TFGrid Studio

Thank you for your interest in contributing! This guide will help you get started.

## Ways to Contribute

### 1. Report Bugs

Found a bug? Help us fix it:

1. Check if the issue already exists in [GitHub Issues](https://github.com/tfgrid-studio/tfgrid-compose/issues)
2. If not, create a new issue with:
   - Clear description of the problem
   - Steps to reproduce
   - Expected vs actual behavior
   - Your environment (OS, versions, etc.)
   - Any relevant logs or screenshots

### 2. Suggest Features

Have an idea? We'd love to hear it:

1. Check [Discussions](https://github.com/orgs/tfgrid-studio/discussions) first
2. Create a new discussion in the "Ideas" category
3. Describe the problem it solves
4. Explain your proposed solution
5. Consider implementation complexity

### 3. Improve Documentation

Documentation is crucial:

- Fix typos and errors
- Add missing information
- Improve clarity
- Add examples
- Write tutorials

### 4. Submit Code

Ready to code? Great!

1. **Fork the repository**
2. **Create a branch** for your feature/fix
3. **Make your changes** following our coding standards
4. **Test thoroughly**
5. **Submit a pull request**

## Pull Request Process

### Before Submitting

- [ ] Code follows existing style
- [ ] Changes are well-tested
- [ ] Documentation is updated
- [ ] Commit messages are clear
- [ ] No unrelated changes included

### Pull Request Template

```markdown
## Description
[Clear description of what this PR does]

## Motivation
[Why is this change needed?]

## Changes
- [List of changes made]

## Testing
[How was this tested?]

## Related Issues
Fixes #[issue number]
```

### Review Process

1. Maintainers will review your PR
2. Address any requested changes
3. Once approved, it will be merged
4. You'll be credited as a contributor!

## Development Setup

### TFGrid Compose

```bash
# Clone the repo
git clone https://github.com/tfgrid-studio/tfgrid-compose
cd tfgrid-compose

# Install
make install

# Run tests
make test

# Check style
make lint
```

### TFGrid AI Agent

```bash
# Clone the repo
git clone https://github.com/tfgrid-studio/tfgrid-ai-agent
cd tfgrid-ai-agent

# See README for setup
```

## Coding Standards

### General

- Write clear, readable code
- Add comments where needed
- Follow existing patterns
- Keep changes focused
- Test your changes

### Bash Scripts

- Use shellcheck
- Follow Google Shell Style Guide
- Add error handling
- Include usage documentation

### Python (if applicable)

- Follow PEP 8
- Use type hints
- Write docstrings
- Add unit tests

### Markdown

- Use clear headings
- Keep lines under 120 characters
- Include code examples
- Link to relevant docs

## Commit Messages

Write clear commit messages:

```
feat: add support for k3s auto-scaling
fix: resolve SSL certificate renewal issue
docs: update gateway pattern README
test: add integration tests for deployment
refactor: simplify network configuration
```

**Format:**
- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation
- `test:` - Tests
- `refactor:` - Code refactoring
- `chore:` - Maintenance

## Getting Help

Need help contributing?

- [GitHub Discussions](https://github.com/orgs/tfgrid-studio/discussions) - Ask questions
- [Documentation](https://docs.tfgrid.studio) - Learn the platform
- [Examples](https://github.com/tfgrid-studio/tfgrid-compose/tree/main/examples) - See working code

## Recognition

All contributors are recognized in:
- Repository contributors list
- Release notes
- Community acknowledgments

## License

By contributing, you agree that your contributions will be licensed under the same license as the project (Apache 2.0 for FOSS repositories).

---

**Thank you for contributing to TFGrid Studio!** 🚀

Your contributions help build the decentralized web.
