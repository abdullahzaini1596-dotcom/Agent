# README for the API Project

# API Project

This project is a Python API built using the uv framework. It follows a flat package structure and is designed to be easy to set up and run.

## Project Structure

```
api/
├── app/                # Contains the application code
│   ├── __init__.py     # Marks the app directory as a package
│   └── main.py         # Entry point of the application
├── .env.example         # Template for environment variables
├── .gitignore           # Specifies files to be ignored by Git
├── .python-version      # Specifies the Python version for the project
├── README.md            # Documentation for the project
├── pyproject.toml       # Project configuration file
└── uv.lock              # Dependency lock file
```

## Getting Started

To get started with this project, follow these steps:

1. **Clone the repository**:
   ```
   git clone <repository-url>
   cd api
   ```

2. **Install dependencies**:
   Use the `uv` tool to install the necessary dependencies:
   ```
   uv sync
   ```

3. **Set up environment variables**:
   Copy the `.env.example` file to `.env` and fill in the required values:
   ```
   cp .env.example .env
   ```

4. **Run the application**:
   Start the API using the following command:
   ```
   uv run --env-file .env python -m app.main
   ```

5. **Access the API**:
   The API will be running at `http://localhost:8000` (or the specified port).

## Testing

To run tests, use the following command:
```
uv run pytest
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.