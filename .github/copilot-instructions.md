# Copilot Instructions (Python)

## General
- Prefer small, readable functions and clear naming.
- Keep changes minimal and focused on the request.

## Project Structure
- Source code lives in the `src/` directory.
- Tests live in the `tests/` directory.

## Testing
- Use `xUnit` as the test framework.
- Name tests `*Tests.cs`.
- The names of test functions should describe the behavior being tested, e.g., `Returns_Correct_Sum()`.
- No comments in tests, the test name should be descriptive enough.
- Don't change existing tests unless necessary to fix a bug or add coverage for new code.
- Either change tests or code, but not both at the same time. It is not possible that a system validates or falsifies itself.

## Documentation

- Add brief comments only when the intent is not obvious.
- Use docstrings to document functions, classes, and modules.
- Use type hints for function parameters and return types.
- The language the documentation is written is English.

