# 🌶️ Framework Flavors (Ecosystem Specifics)

Tailored recipes matching specific runtime environments and language constraints.

---

### 🐍 Flavor 1: The FastAPI & Pydantic Roast (Python)
* **Ingredients:** A legacy Python dict/JSON layout, `pytest` framework.
* **Preparation Instructions:**
```text
Act as an expert Python Backend Engineer. We need to create a secure endpoint based on this model context.

Follow these culinary guidelines:
1. PREP: Create a strict Pydantic v2 validation schema handling inbound payloads, ensuring type-safety and field aliases where necessary.
2. BAKE: Wrap this schema into a clean FastAPI router using explicit dependency injection (`Depends`) for database sessions or security scopes.
3. FLAMBÉ: Generate an asynchronous service layer utilizing modern async/await syntax to handle data persistence.
4. TASTE TEST: Spin up a companion test file using HTTPClient inside `pytest` to guarantee all edge-cases return 200 OK or 422 Unprocessable Entity perfectly.
```

### ☕ Flavor 2: The TypeScript & Type-Safe Soufflé (Node.js)
* **Ingredients:** Strict compiler configuration (`tsconfig.json`), `vitest` or `jest`.
* **Preparation Instructions:**
```text
Act as a Principal Frontend/Node.js Architect. We are building a robust utility module in TypeScript.

Follow these strict steps:
1. MISE EN PLACE: Inspect our project's tsconfig.json to match code emission and module resolutions guidelines.
2. SEASONING: Declare explicit interfaces or types for all domain models. Avoid the use of `any` at all costs; use generics (`<T>`) or `unknown` where abstraction is required.
3. COOKING: Write the implementation module ensuring data immutability (use `readonly` where appropriate).
4. REFINING: Add explicit custom error boundaries ensuring asynchronous promise rejections are handled safely.
```
