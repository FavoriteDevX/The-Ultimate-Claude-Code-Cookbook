<p align="center">
  <img width="410" height="300" alt="image" src="https://github.com/user-attachments/assets/4cc300e3-a146-476e-a549-df87be48b563" />
</p>

# 🍳 The Ultimate Claude Code Cookbook

Welcome to **The Ultimate Claude Code Cookbook**! This is a curated collection of production-grade recipes, prompt injections, and automation configurations explicitly tailored for Anthropic's **Claude Code** CLI. 

We treat software engineering like high gastronomy. Below, you will find a menu of pre-engineered prompts structured with **Ingredients (Requirements)**, **Preparation Steps (Systemic Workflows)**, and **Estimated Token Simmering**.

---

## 🛠️ Kitchen Setup (Core Configurations)

Before executing any recipe, your workstation must be properly prepped with the right tools and global constraints.

### 📜 The Master Menu (`.clauderules`)
Place this file at the root of your repository. Claude Code automatically scans it before prepping any meal to ensure coding standards are strictly enforced.

```markdown
# Global Kitchen Rules
- Always taste-test (run the test suite) before serving changes to production.
- Keep portions small: no function should exceed 80 lines of code.
- Never leave trash in the kitchen: mock all API credentials and secrets.
- Use Conventional Commits formatting to label all shipped deliverables.
- If a terminal command fails twice, stop the stove and ask the Head Chef (User).
```

---

## 🫒 Appetizers (Quick Terminal Commands)

Lightweight command-line commands for instant workspace hygiene and minor code polish.

### 🧼 The Sautéed Workspace Clean-up
* **Description:** Sweeps away dead imports, legacy console logs, and syntax dust across your current active files.
* **The Command:**
```bash
claude "Inspect our active staging files. Safely prune all unused imports, remove commented-out console/print debugging statements, run the automated formatter, and verify the linter yields zero warnings."
```

### 📦 The "Express Delivery" Commit
* **Description:** Autonomously analyzes your current diffs, writes standard git syntax, and pushes to your upstream branch.
* **The Command:**
```bash
claude "Run a git diff to inspect our freshly prepared code. Craft a concise, descriptive commit message matching Conventional Commits standards, execute the commit locally, and push it upstream."
```

---

## 🥩 Main Courses (Robust Automation Workflows)

Heavy-duty, multi-step prompt recipes designed to handle major architectural refactoring and deep bug hunting.

### 🏗️ Recipe 1: Legacy Code Flambé (Modernization)
* **Description:** Upgrading an outdated, monolithic module into an optimized, highly typed modern component.
* **Ingredients (Requirements):** 
  - `[PATH_TO_OLD_MODULE]`: The legacy file targeted for reconstruction.
  - `[TARGET_TECH_STACK]`: Your preferred framework/language flavor (e.g., TypeScript, FastAPI, Go).
  - `[NEW_MODULE_NAME]`: The destination filename for the clean implementation.
* **Preparation Instructions:**
```text
Act as a Principal Software Architect. Your task is to modernize the legacy module at [PATH_TO_OLD_MODULE] into [TARGET_TECH_STACK].

Execute this preparation sequence carefully:
1. MISE EN PLACE: Read the legacy file entirely. Map out all its public API contracts, hidden side-effects, and internal logic.
2. PORTIONING: Isolate shared sub-components and extract them into clean, standalone utility functions.
3. COOKING: Rewrite the entire module in a brand-new file named [NEW_MODULE_NAME]. Implement strict type checking, robust error handling, and inline documentation.
4. TASTE TEST: Update the project's internal import routes to point to the new file, run the compiler, and ensure it builds with zero errors.
5. CLEAN UP: Safely delete or archive the old file once compilation succeeds.
```

### 🐛 Recipe 2: Test-Driven Bug Poaching (TDD)
* **Description:** Finding, reproducing, and neutralizing a production defect using a rigorous Test-Driven approach.
* **Ingredients (Requirements):**
  - `[BUG_SYMPTOMS]`: Detailed error stack-traces or user bug reports.
  - `[TEST_SUITE_COMMAND]`: The terminal command used to trigger execution (e.g., `npm test`, `pytest`).
* **Preparation Instructions:**
```text
We have received reports that the system fails when: [DESCRIBE_BUG_SYMPTOMS].

Follow this strict Test-Driven Development recipe to fix it:
1. SCAN: Locate the source files handling this logic and read their internal structures.
2. SOUR THE DISH: Write a brand new unit test within our test suite that specifically replicates this bug scenario. Run [TEST_SUITE_COMMAND] and confirm this new test explicitly FAILS.
3. ADJUST SEASONING: Modify the core implementation layer with the minimal amount of changes required to make the failing test pass.
4. FULL BANQUET INSPECTION: Run the global [TEST_SUITE_COMMAND] suite across the entire repository to confirm no collateral regressions were introduced.
5. SERVE: Write a quick summary explaining why the bug happened and how your fix permanently patches it.
```

---

## 🍨 Desserts (Boilerplate Generation)

Quick, highly rewarding recipes to auto-generate entire architecture blocks out of single raw assets.

### ⚡ Schema-to-API Soufflé
* **Description:** Takes a raw database schema layout and spins up a ready-to-serve REST/GraphQL endpoint with validation layers.
* **Ingredients (Requirements):**
  - `[PATH_TO_SCHEMA_FILE]`: The raw file holding your database or data models.
  - `[VALIDATION_LIBRARY]`: Your framework validation schema runner (e.g., Zod, Pydantic).
* **Preparation Instructions:**
```text
Analyze the architectural model definition found inside [PATH_TO_SCHEMA_FILE].

Generate a complete, production-ready CRUD controller system using these constraints:
- Construct valid endpoints for GET, POST, PUT, and DELETE operations.
- Inject a strict validation middleware schema using [VALIDATION_LIBRARY] to intercept incoming traffic.
- Map out accurate semantic HTTP status codes (200/201 for success, 400 for bad payloads, 404 for missing entities, 500 for unhandled crashes).
- Automatically bake mock data factories into a side file to make unit testing this endpoint seamless.
```

---

## 🛡️ Kitchen Safety (Token & Budget Control)

Operating an autonomous CLI agent requires proper stove guards. Use these guidelines to avoid setting your API budget on fire.

* **Don't Overcrowd the Pot:** Avoid asking Claude vague questions like `"optimize my repository"`. It will ingest thousands of lines of context, bloating your API bill. Always pinpoint your targets using explicit filepaths.
* **Prevent Over-Boiling (The Kill Switch):** If Claude gets trapped in an infinite recursive testing loop or repeatedly fails a command, do not wait for the context to fill up. Instantly execute a hard stop using **`Ctrl + C`**.
* **Check the Bill:** Claude Code displays your exact token consumption after complex processes. Treat this as your kitchen receipt to track your computational overhead.
