# Naveen Kumar Chilakala

Software engineer, 8+ years in production. **Python · Rust · TypeScript · Java.**
I mostly work on hard bugs, performance, refactors, and features built end to end, and I measure before and after.

## Projects

**[digi-setu-editor](https://github.com/ChilakalaNaveenKumar/digi-setu-editor)** (Rust · Python · TypeScript)
Desktop and web editor. A Rust (Tauri 2) shell supervises a Python FastAPI process and a Vue UI. The Rust I wrote is in [`desktop/src-tauri/src`](https://github.com/ChilakalaNaveenKumar/digi-setu-editor/tree/main/desktop/src-tauri/src):
- `sidecar.rs`: process supervisor with free-port allocation, a health-check wait, a watchdog that restarts with exponential backoff, and an `Arc<AtomicBool>` shutdown flag
- `secure_storage.rs`: OS keychain sessions with a file fallback · `updater.rs`: signed auto-update · `build.rs`: fails the build if a live secret is in the environment
- Found two startup race conditions; the ready signal went from **+9.5 s to +10 ms**. Removed a 250 MB / 19k-file copy so Windows installs went from **2–5 min to about 3 s**.

**[kit-assembly-eval](https://github.com/ChilakalaNaveenKumar/kit-assembly-eval)** (Python)
A code-graded benchmark: can a model assemble a working machine from loose SVG parts? It has 6 kits, 3 difficulty levels and 162 graded builds. Reference solutions must pass the grader, and a re-grade script shows the saved results never change. Best model: 72% with the joints listed, 33% without.

**[hello-again-coding-challange](https://github.com/ChilakalaNaveenKumar/hello-again-coding-challange)** (Python · Django)
Compares slow and optimised list/search APIs over 3 million rows using indexes, `select_related`/`prefetch_related` and subqueries, with a dashboard showing the response times.

## Work
LifeVantage (via Computer Power Group), 2024–now: Shopify Plus checkout and subscription features in TypeScript, plus Python developer tooling.
Keylane: React and Java Spring Boot. Modak Analytics (GSK, AbbVie, Humana): Vue and Node.js.
Most of my work commits live in private company repos.

M.S. Computer Science, Auburn University at Montgomery
