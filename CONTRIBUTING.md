# Contributing to Financial Sentiment Analysis

Thank you for your interest in contributing to this project! This document provides a repository map and guidelines to help you get started.

## 📍 Repository Map

### Directory Structure Overview

```
financial-sentiment-week1/
│
├── 📓 notebooks/              # Jupyter notebooks for analysis
│   ├── 01_eda_analysis.ipynb  # Exploratory Data Analysis
│   ├── 02_quantitative_analysis.ipynb  # Quantitative metrics
│   ├── README.md              # Notebook-specific documentation
│   └── reports/               # Generated visualizations and reports
│
├── 📁 data/                   # Data storage
│   ├── raw/                   # Original, unprocessed data
│   │   ├── stocks/            # Stock price CSV files
│   │   └── row/               # Raw analyst ratings
│   └── processed/             # Cleaned and transformed data
│
├── 🔧 scripts/                # Utility scripts and helpers
│   └── README.md              # Script documentation
│
├── 💻 src/                    # Source code modules (future)
│   └── __init__.py
│
├── 🧪 tests/                  # Unit and integration tests
│   └── __init__.py
│
├── 📊 reports/                # Additional analysis reports
│   └── README.md
│
├── 📄 requirements.txt        # Python dependencies
├── 📖 README.md               # Main project documentation
└── 📝 CONTRIBUTING.md         # This file
```

### Key Files & Their Purposes

| File/Directory | Purpose | When to Modify |
|---------------|---------|----------------|
| `notebooks/01_eda_analysis.ipynb` | Initial data exploration | When adding new EDA features |
| `notebooks/02_quantitative_analysis.ipynb` | Financial metrics analysis | When adding new calculations |
| `data/raw/` | Original data files | **Never modify** - read-only |
| `data/processed/` | Cleaned data outputs | When preprocessing data |
| `scripts/` | Reusable utility functions | When creating helper functions |
| `requirements.txt` | Python package dependencies | When adding new libraries |
| `README.md` | Project documentation | When updating project info |

## 🚀 Getting Started

### 1. Setup Development Environment

```bash
# Clone the repository
git clone <repository-url>
cd financial-sentiment-week1

# Create and activate virtual environment
python -m venv .venv

# Windows
.venv\Scripts\activate

# macOS/Linux
source .venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

### 2. Choose Your Contribution Area

- **Data Analysis**: Work in `notebooks/` directory
- **Utility Functions**: Add to `scripts/` directory
- **Testing**: Add tests to `tests/` directory
- **Documentation**: Update README files
- **Bug Fixes**: Identify and fix issues in existing code

## 📝 Coding Standards

### Python Style Guide

- Follow **PEP 8** style guidelines
- Use **type hints** for function parameters and return values
- Maximum line length: **100 characters**
- Use **4 spaces** for indentation (no tabs)

### Function Documentation

All functions should include docstrings in Google style:

```python
def example_function(param1: str, param2: int) -> pd.DataFrame:
    """
    Brief description of what the function does.
    
    Args:
        param1: Description of first parameter
        param2: Description of second parameter
        
    Returns:
        Description of return value
        
    Raises:
        ValueError: When parameter is invalid
        
    Example:
        >>> result = example_function("test", 42)
        >>> print(result)
    """
    # Implementation here
    pass
```

### Inline Comments

- Use comments to explain **why**, not **what**
- Keep comments concise and relevant
- Update comments when code changes
- Use `# TODO:` for future improvements

### Example:

```python
# Good: Explains why
# Use robust path resolution to handle different working directories
data_path = resolve_data_path(DATA_RELATIVE_PATH)

# Bad: States the obvious
# Get the data path
data_path = resolve_data_path(DATA_RELATIVE_PATH)
```

## 🔄 Workflow

### 1. Create a Branch

```bash
git checkout -b feature/your-feature-name
# or
git checkout -b fix/bug-description
```

### 2. Make Your Changes

- Write clean, documented code
- Test your changes locally
- Update relevant documentation
- Follow the coding standards above

### 3. Commit Your Changes

Use clear, descriptive commit messages:

```bash
git commit -m "Add: sentiment correlation analysis function"
git commit -m "Fix: handle NaN values in time series analysis"
git commit -m "Docs: update README with new analysis methods"
```

**Commit Message Prefixes:**
- `Add:` - New feature
- `Fix:` - Bug fix
- `Update:` - Modification to existing feature
- `Docs:` - Documentation changes
- `Refactor:` - Code restructuring
- `Test:` - Adding or updating tests

### 4. Push and Create Pull Request

```bash
git push origin feature/your-feature-name
```

Then create a Pull Request with:
- Clear description of changes
- Reference to related issues (if any)
- Screenshots/visualizations (if applicable)

## 🧪 Testing Guidelines

### Before Submitting

1. **Run notebooks end-to-end**: Ensure all cells execute without errors
2. **Check data integrity**: Verify outputs are reasonable
3. **Validate visualizations**: Ensure charts render correctly
4. **Test edge cases**: Handle missing data, empty datasets, etc.

### Test Checklist

- [ ] All cells execute successfully
- [ ] No warnings or errors in output
- [ ] Visualizations generate correctly
- [ ] Documentation is updated
- [ ] Code follows style guidelines

## 📊 Data Handling

### Data Files

- **Never commit large data files** to git
- Use `.gitignore` to exclude data files
- Document data sources in README
- Keep raw data in `data/raw/` (read-only)
- Save processed data to `data/processed/`

### Data Processing

- Always validate data before processing
- Handle missing values explicitly
- Document data transformations
- Preserve original data integrity

## 🐛 Reporting Issues

When reporting bugs or requesting features:

1. **Check existing issues** first
2. **Use clear titles** describing the issue
3. **Provide context**: What were you trying to do?
4. **Include error messages** and tracebacks
5. **Add reproduction steps** if applicable
6. **Attach relevant files** (screenshots, data samples)

## 💡 Feature Requests

We welcome feature suggestions! When proposing new features:

1. **Describe the use case**: Why is this feature needed?
2. **Propose implementation**: How should it work?
3. **Consider alternatives**: Are there existing solutions?
4. **Discuss impact**: How does it affect existing code?

## 📚 Additional Resources

- [PEP 8 Style Guide](https://pep8.org/)
- [Google Python Style Guide](https://google.github.io/styleguide/pyguide.html)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Jupyter Notebook Best Practices](https://www.dataquest.io/blog/jupyter-notebook-tips-tricks-shortcuts/)

## ❓ Questions?

If you have questions or need help:

1. Check the README.md for project overview
2. Review existing code for examples
3. Open an issue with your question
4. Check notebook comments and docstrings

---

**Thank you for contributing!** 🎉

