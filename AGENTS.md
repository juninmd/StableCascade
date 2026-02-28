```markdown
# AGENTS.md File Guidelines

These guidelines are designed to ensure the consistent, maintainable, and high-quality development of the AGENTS repository. Adherence to these principles will significantly improve the long-term stability and usability of the codebase.

## 1. DRY (Don't Repeat Yourself)

*   All logic and data structures should be encapsulated within single, well-defined modules.
*   Avoid duplication of code across multiple files.  If a functionality needs to be reused, it should be extracted into a separate module.
*   Whenever possible, leverage existing components and libraries to reduce code duplication.

## 2. KISS (Keep It Simple, Stupid)

*   Strive for simplicity in design and implementation.
*   Prioritize readability and maintainability over rapid prototyping.
*   Keep functions and classes as small and focused as possible.
*   Avoid unnecessary complexity.

## 3. SOLID Principles

*   **Single Responsibility Principle:** Each class/module should have one and only one reason to change.
*   **Open/Closed Principle:**  Systems should be extensible without modifying their core implementation.  New functionality should be added through new classes, not modifications to existing ones.
*   **Liskov Substitution Principle:**  Subclasses should be substitutable for their base classes without altering the correctness of the system.
*   **Interface Segregation Principle:** Clients should not be forced to satisfy multiple interfaces.
*   **Dependency Inversion Principle:**  High-level modules (interfaces) should be replaced by low-level modules (implementations).

## 4. YAGNI (You Aren't Gonna Need It)

*   Only implement functionality that is explicitly required *now*.  Avoid adding features without a clear, immediate need.
*   Refactor existing code to remove unneeded complexity.

## 5. Code Style & Formatting

*   **Indentation:** Use 2 spaces for indentation.
*   **Line Length:** Maximum 120 characters per line.
*   **Naming Conventions:** Follow standard Python naming conventions (PEP 8).
*   **Comments:** Provide concise, helpful comments where necessary, but avoid excessive commenting.  Focus on explaining *why* not *what*.

## 6. File Size & Code Coverage

*   **Maximum File Size:** 180 lines of code.
*   **Minimum Test Coverage:** 80%. All code must be covered by at least 80% tests.

## 7. Testing & Validation

*   **Mocking:** All tests must be written using mocks and stubs, *not* to actually generate simulated data. The goal is to isolate the code being tested.
*   **Unit Tests:** Focus on testing individual functions and classes in isolation.
*   **Integration Tests:**  Tests should verify the interaction between multiple components or modules.
*   **Regression Tests:**  Ensure that new changes do not break existing functionality. Automated regression tests are critical.

## 8. Development Workflow

*   **Version Control:** Use Git with a well-defined branching strategy.
*   **Code Reviews:**  All code must be reviewed by at least one other developer before merging.
*   **Documentation:**  Clear documentation is required for all modules and functions.
*   **Refactoring:** Regularly refactor code to improve its design and maintainability.

## 9.  Specific Constraints (Optional -  Consider adding as needed)

*   [Example Constraint 1:  Data structure used must be efficient for certain operations.]
*   [Example Constraint 2:  API endpoints should follow a specific pattern.]
*   [Example Constraint 3:  No external dependencies are allowed.]

## 10.  Further Considerations

*   Explore using dependency injection (DI) to improve testability and modularity.
*   Design for scalability.  Consider potential future growth and maintainability.
*   Prioritize clarity and readability.  Ensure the code is easy to understand and modify.
```