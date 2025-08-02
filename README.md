# [Joystick Gremlin Action Copier](https://rolex20.github.io/JG-Action-Copier/JG_ActionCopier.html)

A browser-based tool to copy and paste actions, curves, and macros between Joystick Gremlin XML profiles with surgical precision.

This application was created through a unique collaboration between a human software architect and multiple advanced AI models, showcasing the power of expert-led context engineering over simple prompting.

---

## About The Project & The AI Collaboration

This project was developed using advanced context engineering techniques. The human architect provided the AI with detailed specifications, real-world XML samples, schematics, and iterative feedback, orchestrating a collaborative workflow. The development journey involved multiple stages and AIs:

1.  **Initial Creation (Gemini & Claude):** The first version was created to handle basic copying.
2.  **Initial Bug Fixes (The User & Abacus):** The user identified a critical data-loss bug, which was fixed by adding safe, "add-only" logic.
3.  **The Architectural Flaw:** The user then correctly diagnosed that "add-only" was insufficient, as it could create functional conflicts (e.g., two remaps on one axis).
4.  **Final Architecture (The User & Abacus):** The application was completely re-architected to provide the necessary granular control, turning it from a simple utility into a robust, professional-grade tool.

This project demonstrates how human expertise can guide AI to solve complex, real-world problems far beyond simple "snake game" examples.

---

## Why This Application Exists

If you’re a flight simulation enthusiast, you know the pain of managing dozens of Joystick Gremlin (JG) profiles. Recreating macros, curves, or actions by hand is tedious and error-prone, and editing XML directly is risky.

**Joystick Gremlin Action Copier** solves this by letting you load all your JG XML profiles at once, building a searchable library of every action you've ever created. You can visually browse, find, and copy actions with precision, choosing to either add them as new or replace existing ones to avoid conflicts.

**Key Benefits:**
- **Massive time saver:** No more recreating complex actions by hand.
- **Error reduction:** No more risky manual XML edits.
- **Granular Control:** Choose to **add** a new action or precisely **replace** an existing one.
- **Conflict Prevention:** Avoid creating broken profiles by replacing, not just adding, conflicting actions like remaps.
- **Bulk management:** Handles dozens of profiles and thousands of actions at once.
- **Safe & User-friendly:** A single, portable HTML file—no installation, no dependencies.

---

## Features

- **Load Multiple Source Profiles:** Import any number of source XML profiles.
- **Granular Container Selection:** Browse and select individual action containers within each axis or button.
- **Add or Replace Functionality:** Explicitly choose to add a container to a target or replace an existing one.
- **Intelligent Preview:** The preview modal clearly shows whether you are about to ADD or REPLACE and displays the relevant XML for confirmation.
- **Robust Tree-Preserving Search:** Instantly filter the source library; the search will always show the full path to any matching item.
-   **Seamless Workflow:** After an operation, the UI intelligently refreshes, allowing for multiple, consecutive copy/replace actions without starting over.
- **Detailed Operation Log:** Track all `[ADD]` and `[REPLACE]` actions performed in the current session.
- **Safe Save:** Download the updated target profile as a new, validated XML file.
- **100% Client-Side:** No installation, no dependencies, no server. Your data never leaves your computer.

---

## Usage

1.  **Open the App:**  
    Download and open JG_ActionCopier.html(https://rolex20.github.io/JG-Action-Copier/JG_ActionCopier.html) in your web browser.

2.  **Load Profiles:**  
    - Select one or more **source** XML profiles.
    - Select a single **target** XML profile.

3.  **Browse and Select:**  
    - In the "Source Library" panel, expand the trees to find and select the specific **container** you wish to copy.
    - In the "Target Destinations" panel, the corresponding inputs will appear. Expand the desired target.

4.  **Choose Operation (Add or Replace):**
    - To **add** the source container, select the `[+] Add as New Container` option in the target.
    - To **replace** an existing container, select that specific container in the target list.

5.  **Preview and Confirm:**  
    - Click "Preview Operation". A modal will appear, clearly stating the action (ADD/REPLACE) and showing the XML.
    - Click "Confirm" to perform the operation.

6.  **Save Changes:**  
    - After performing one or more operations, enter an output filename and click "Save Modified Profile".

---

## Credits

-   **Human Architect & Context Engineer:** rolex (The user who guided the project).
-   **AI Development Team:**
    -   **Gemini & Claude:** Performed initial application scaffolding and feature implementation.
    -   **ChatGPT:** Wrote the initial draft of the README.
    -   **Gemini 2.5 Pro with Google AI Studio:** Performed the final, major architectural overhaul (v2.0), implemented the granular add/replace logic, and conducted the final code review and perfectioning (v2.1).

---

## Requirements

- Any modern web browser (Chrome, Edge, Firefox, Safari)
- Joystick Gremlin XML profiles

---

## License

MIT License
