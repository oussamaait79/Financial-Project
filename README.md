# Robot Framework Test Automation Project

This project contains automated tests using Robot Framework with Selenium Library.

## Project Structure

```
├── scripts/
│   ├── import_data.py      # Data import script
│   └── clean_data.py       # Data cleanup script
├── tests/
│   ├── resources/
│   │   └── common.robot    # Common keywords and variables
│   └── test_suite.robot    # Test cases
├── .env.example            # Example environment variables
├── requirements.txt        # Python dependencies
└── package.json           # Node.js dependencies
```

## Setup

1. Install Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Install Node.js dependencies:
   ```bash
   npm install
   ```

3. Copy `.env.example` to `.env` and update with your configuration:
   ```bash
   cp .env.example .env
   ```

## Available Scripts

- Import test data:
  ```bash
  npm run import-data
  ```

- Run tests:
  ```bash
  npm run run-tests
  ```

- Clean up test data:
  ```bash
  npm run clean-data
  ```

## Pipeline Structure

The automation is divided into three main pipelines:

1. Data Import Pipeline
   - Imports necessary test data
   - Sets up the test environment

2. Test Execution Pipeline
   - Runs the Robot Framework tests
   - Generates test reports

3. Data Cleanup Pipeline
   - Cleans up test data
   - Resets the environment

## Best Practices

- Keep test cases independent and atomic
- Use page objects for better maintainability
- Store sensitive data in environment variables
- Regular cleanup of test data
- Maintain clear documentation