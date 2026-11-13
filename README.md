# TCS JFLAP Self Learning

**Name :** Dheer Java  
**Class/Roll No:** D12B-21  
**Subject:** Theory of Computer Science (TCS)  
**Tool:** JFLAP  

---

## About JFLAP

**JFLAP** (Java Formal Languages and Automata Package) is an interactive educational software tool designed for experimenting with formal languages and automata theory. It provides a visual and interactive environment to design, simulate, and analyze foundational computational models studied in Computer Science.

### Key Capabilities:
- **Graphical Automata Design:** Construct and visually lay out state diagrams for finite automata, pushdown automata, and Turing machines.
- **Interactive Simulation:** Execute inputs using Single Step, Fast Run, and Multiple Run (batch testing) to evaluate acceptance and rejection behavior.
- **Formal Grammar Tools:** Define regular and context-free grammars, test derivations, eliminate ambiguity, and transform grammars into normal forms.
- **Parsing Algorithms:** Construct and visualize parsing tables for LL(1) top-down parsing and the Cocke–Younger–Kasami (CYK) dynamic programming algorithm.
- **Automated Conversions:** Step through equivalence algorithms, including Regular Expression to NFA/DFA, Grammar to DFA, CFG to CNF, and CFG to NPDA.

---

## Topics Covered

This assignment uses 30 JFLAP files to practice core Theory of Computer Science models. Each file focuses on one construction, conversion, parser, or machine behavior.

The examples use numeric input symbols where applicable, mainly `0` and `1`. Uppercase grammar variables and stack markers remain unchanged.

### Topics Covered

1. **Deterministic Finite Automata (DFA):**
   - Counting conditions, parity, divisibility, and pattern tracking.
   - Prefix, suffix, substring, and exact-occurrence recognition.

2. **Non-Deterministic Finite Automata (NFA):**
   - Branching paths and state guessing.
   - Recognition of patterns with multiple possible paths.

3. **Regular Expressions (RE) & Regular Grammars:**
   - Regular-language specification.
   - Right-linear grammars and conversions among expressions, grammars, and finite automata.

4. **Finite State Machines with Output (Transducers):**
   - **Mealy Machines:** Output determined by current state and input.
   - **Moore Machines:** Output attached to the current state.

5. **Context-Free Grammars (CFG):**
   - Generating languages such as `0^n1^n`.
   - Modeling structural patterns such as balanced strings and palindromes.

6. **Chomsky Normal Form (CNF):**
   - Transforming context-free grammars into restricted rules such as `A -> BC` and `A -> 0`.

7. **Pushdown Automata (PDA / NPDA):**
   - Stack-based recognition of context-free languages.
   - Acceptance by final state or empty stack.
   - CFG and NPDA conversion.

8. **Parsing Algorithms:**
   - **LL(1) Parsing:** First and Follow sets plus predictive parse tables.
   - **CYK Parsing:** Dynamic-programming membership checks using CNF grammars.

## JFLAP Files

| # | Topic | File | Main activity |
|---:|---|---|---|
| 1 | Deterministic Finite Automata | `01_deterministic_finite_automata.jff` | DFA ending in `01` |
| 2 | Nondeterministic Finite Automata | `02_nondeterministic_finite_automata.jff` | NFA ending in `01` |
| 3 | NFA to DFA Conversion | `03_nfa_to_dfa_conversion.jff` | Subset construction |
| 4 | DFA Minimization | `04_dfa_minimization.jff` | Merge equivalent states |
| 5 | DFA to Regular Grammar | `05_dfa_to_regular_grammar.jff` | Convert DFA to grammar |
| 6 | DFA to Regular Expression | `06_dfa_to_regular_expression.jff` | Derive a regular expression |
| 7 | Combining Automata | `07_combining_automata.jff` | Combine automata behavior |
| 8 | Regular Expression | `08_regular_expression.jff` | Test a regular expression |
| 9 | Regular Expression to DFA | `09_regex_to_dfa.jff` | Convert expression to DFA |
| 10 | Regular Expression Identities | `10_regular_expression_identities.jff` | Compare equivalent expressions |
| 11 | Regular Grammar | `11_regular_grammar.jff` | Generate a regular language |
| 12 | Regular Grammar to DFA | `12_regular_grammar_to_dfa.jff` | Convert grammar to DFA |
| 13 | DFA and Grep | `13_dfa_grep_abb.jff` | Model a search pattern |
| 14 | Mealy Machine | `14_mealy_detect_01.jff` | Detect `01` with output |
| 15 | Moore Machine | `15_moore_detect_01.jff` | Detect `01` by state output |
| 16 | Context-free Grammar | `16_context_free_grammar.jff` | Generate a CFG language |
| 17 | Pushdown Automaton | `17_pushdown_automaton.jff` | Recognize `0^n1^n` |
| 18 | NPDA to CFG | `18_npda_even_palindrome.jff` | Convert an NPDA |
| 19 | CFG to NPDA | `19_cfg_balanced_parentheses.jff` | Convert a CFG |
| 20 | CFG with Single Symbols | `20_cfg_single_symbols.jff` | Trace unit productions |
| 21 | CFG with Multiple Symbols | `21_cfg_multiple_symbols.jff` | Trace multi-symbol rules |
| 22 | CFG User-Controlled Parse | `22_cfg_error_parse.jff` | Step through derivation |
| 23 | LL Parsing | `23_ll_parsing.jff` | Build LL parse table |
| 24 | LR Parsing | `24_lr_parsing.jff` | Explore LR parsing |
| 25 | CYK Parsing | `25_cyk_parsing.jff` | Fill a CYK table |
| 26 | One-Tape Turing Machine | `26_one_tape_turing_machine.jff` | Rewrite tape symbols |
| 27 | Multi-Tape Turing Machine | `27_multi_tape_turing_machine.jff` | Copy input to another tape |
| 28 | Turing Machine Building Block | `28_turing_building_block.jff` | Move to the first blank |
| 29 | Unrestricted Grammar | `29_unrestricted_grammar.jff` | Derive a type-0 language |
| 30 | L-System | `30_lsystem_simple.jff` | Expand rewriting rules |

---

## How to Open and Run

### 1. Prerequisites
- **Java Runtime Environment (JRE):** Java 8, 11, or newer installed on your machine.
- **JFLAP:** `JFLAP7.1.jar` executable.

To verify Java is installed, run:
```bash
java -version
```

### 2. Launching JFLAP
Open a terminal in the folder containing `JFLAP7.1.jar` and run:
```bash
java -jar JFLAP7.1.jar
```
*Alternatively, you can double-click `JFLAP7.1.jar` directly in File Explorer.*

### 3. Opening Assignment Files
1. In the JFLAP main menu, click **File** $\to$ **Open** (or press `Ctrl + O`).
2. Navigate to this directory and select any `.jff` file to load its diagram, grammar, or expression into the workspace.

### 4. Running and Testing Models

#### For Finite Automata & Pushdown Automata (DFA, NFA, PDA):
- **Batch Testing (Multiple Run):**
  1. Click **Input** $\to$ **Multiple Run**.
  2. Enter test strings into the input column.
  3. Click **Run Inputs** to see instant `Accept` or `Reject` verdicts.
- **Step-by-Step Visualization:**
  - Click **Input** $\to$ **Step with State** (or **Step by State**) to step through state transitions symbol-by-symbol with active stack/state inspection.
- **Fast Run:**
  - Click **Input** $\to$ **Fast Run** for quick single-string verification.

#### For Mealy & Moore Machines:
1. Click **Input** $\to$ **Multiple Run** (or **Fast Run**).
2. Enter an input sequence to view the generated synchronous output sequence alongside each transition.

#### For Grammars (CFG, LL(1), CYK):
- **Brute Force Parsing:**
  - Click **Input** $\to$ **Brute Force Parse** $\to$ enter a string to generate its derivation tree.
- **LL(1) Parse Table:**
  - Click **Input** $\to$ **Build LL(1) Parse Table** to inspect First/Follow sets and construct the LL(1) parsing matrix.
- **CYK Parsing:**
  - Click **Input** $\to$ **CYK Parse** $\to$ enter an input string to dynamically fill the triangular parsing table.

#### For Equivalence & Conversions:
- Use the **Convert** menu in JFLAP to step through automated conversions:
  - `Convert` $\to$ `Convert to NFA` / `Convert to DFA` (for Regular Expressions).
  - `Convert` $\to$ `Convert to FA` (for Regular Grammars).
  - `Convert` $\to$ `Transform to CNF` (for CFGs).
  - `Convert` $\to$ `Convert to PDA` (for CFGs).
