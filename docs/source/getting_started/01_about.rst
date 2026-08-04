========================
1. About MARV Platform
========================

**MARV** (*Managed Activities, Review, and Validation*) is an all-in-one platform engineered to transform software developer education.

Why MARV?
---------

Traditional programming tutorials require students to constantly split screen real estate between web browser instructions and terminal windows. This results in frequent context-switching, accidental copy-paste errors, and fragmented learning workflows.

MARV solves this by embedding instructional materials directly into the Visual Studio Code environment as an interactive extension sidebar.

.. note::
   **Core Philosophy:** Developer education should happen where real development takes place—inside an integrated development environment (IDE).

System Architecture
-------------------

MARV connects three fundamental components:

1. **Tutorial Viewer Pane:** Renders rich reStructuredText pages with interactive buttons, callouts, and embedded quizzes.
2. **Editor Workspace:** Holds your project files, source code, and exercise solutions.
3. **Integrated Terminal:** Receives direct commands from tutorial buttons and streams output feedback in real time.

Prerequisites
-------------

Before installing MARV, ensure you have installed:
* **Visual Studio Code:** Version 1.70.0 or higher.
* **Python 3:** Version 3.8 or higher (for Python-based tutorial verifications).
* **Git:** Version 2.20 or higher.
