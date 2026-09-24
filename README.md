# Learning Lean 4 (Under Duress)

Alright, my professor decided I needed to learn this cursed language for a "special academic side quest," so here I am: an undergrad freshman forced to debug mathematical proofs instead of writing normal code.

This repo tracks my personal survival journey through **Lean 4** and formal software verification (honestly, zero expectations of success, but we ball anyway).

---

### Setup & Reproduce (If you hate yourself enough to try)

1. **Install `elan` (The Lean toolchain manager):**
   ```bash
   curl https://raw.githubusercontent.com/leanprover/elan/master/elan-init.sh -sSf | sh
    ```

2. **Clone & Build this repo:**
    ```bash
    git clone https://github.com/whlongg/lean4-verification.git
    cd lean4-verification
    lake update
    lake build
    ```
    *(Note: No heavyweight Mathlib compilation here. We verify algorithms and state machines, not epsilon-delta calculus).*

3. **Core Survival Materials (Read this or suffer):**
    * **The Hitchhiker’s Guide to Logical Verification (LoVe):** [The primary roadmap for this repo.](https://github.com/blanchette/logical_verification_2023)
    * **Functional Programming in Lean:** [Teaching Lean 4 as an actual programming language rather than a math chalkboard.](https://lean-lang.org/functional_programming_in_lean/)
    * **Theorem Proving in Lean 4:** [When things break and the compiler refuses to cooperate.](https://leanprover.github.io/theorem_proving_in_lean4/)

---

### Current Survival Status

- [ ] Understand Dependent Type Theory without getting an aneurysm
- [ ] Stop replacing hard proofs with `sorry`
- [ ] Model an agent routing state machine without breaking the Lean compiler
- [ ] Convince my professor to let me use Python instead

### Verification Roadmap
- [ ] **[1. Functional Core]** → Inductive Types, Pattern Matching, Recursion
- [ ] **[2. Curry-Howard & Logic]** → Propositions-as-Types, Induction, Basic Tactics
- [ ] **[3. Transition System]** → Agent Modeling: State, Action, Transition Relations
- [ ] **[4. Invariant Proofs]** → Formally Proving Deadlock-Freedom & Safe Routing

> **Friendly PSA:** *If you DO NOT want your professor forcing you to retake this cursed shit for a second semester, DO NOT use Codex Ultra Mode lol.*