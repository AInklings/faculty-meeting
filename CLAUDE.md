# General Code Guidelines

- **Indentation**: Use tabs for indentation.
- **String literals**: Prefer single quotes.
- **Semicolons**: Avoid semicolons at the end of statements.
- **Arrow functions**: Prefer implicit returns when possible.
- **Linting**: Run appropriate code linting and formatting tools after making changes to catch style issues.
- **Build verification**: Ensure builds pass before committing.
- **Testing**: Run unit tests (or relevant test suites) before committing to ensure functionality.
- **Runtime checks**: Perform flag or configuration checks inside functions, not at module scope.

- **Never mock in automated tests** – refactor for testability (extract functions/methods) or use simple test doubles or polymorphic substitution if necessary.
- **Defensive coding: fallback values** – be very careful when implementing fallbacks. Masking configuration errors can hide bugs. Document any fallback behavior and prefer loud failures for critical settings.
