# Joystick Gremlin Action Copier

- A browser-based tool to copy and paste actions, curves, and macros between Joystick Gremlin XML profiles.
- This is an app fully created by an AI with context engineering instead of prompt engineering.  Read below why this matters.

---

## About Human Involvement & Context Engineering

- This AI app was not the typical 'write a snake game' to show that everyone can write apps with AI.

- This project was developed using advanced context engineering techniques, not just traditional prompt engineering. I provided the AI with detailed specifications, real-world XML samples, and iterative feedback, orchestrating a collaborative workflow that leveraged both my software engineering expertise and the AI’s capabilities. This approach ensured the final application was robust, user-focused, and precisely tailored to real user needs—demonstrating my ability to manage this type of projects and maximize the productivity of modern AI tools in professional software development.

- Take a look at the word file that was one of the specs provided for context engineering.

- Prompt engineering is about the “what” and “how” of a single message.
  
- Context engineering is about the “who, what, when, where, and why” of the entire session or application, including all relevant background, files, and ongoing state.

---

## Why This Application Exists

If you’re a flight simulation enthusiast with a growing collection of joysticks, throttles, and rudder pedals, you know the pain of managing dozens of Joystick Gremlin (JG) profiles. Each profile is carefully crafted for different hardware and aircraft, but Joystick Gremlin’s GUI does not allow you to copy or replicate macros, curves, or actions between profiles or devices. Recreating these by hand is tedious and error-prone, and editing XML directly is risky.

**Joystick Gremlin Action Copier** solves this problem by letting you load all your JG XML profiles at once, building an internal database of every action, macro, and curve you’ve ever created. You can visually browse, search, and filter these actions—by name, description, or label—across all your files. When you want to copy a macro, curve, or action, you simply select it from the source tree, pick a compatible destination in your target profile, and preview the exact XML changes before confirming. The app ensures you only copy valid actions to valid destinations, and it validates the XML before saving.

**Key Benefits:**
- **Massive time saver:** No more recreating complex actions by hand.
- **Error reduction:** No more risky manual XML edits.
- **Bulk management:** Handles dozens of profiles and thousands of actions at once.
- **Searchable:** Instantly find what you need, even if you don’t remember the ID.
- **Safe:** Always preview and validate before saving.
- **User-friendly:** All in a single, portable HTML file—no installation, no dependencies.

---

## Features

- **Load Multiple Source Profiles:** Import any number of source XML profiles at once.
- **Target Profile Editing:** Select a single target profile to modify.
- **Visual Tree Navigation:** Browse devices, axes, and buttons in a clear, expandable tree view.
- **Live Search:** Instantly filter source actions by device, name, or description.
- **Preview Before Copy:** See exactly what will be copied and where, with a side-by-side XML preview modal.
- **Safe Copying:** Confirm or cancel each copy operation before making changes.
- **Operation Log:** Track all copy actions performed in the current session.
- **Save Modified Profile:** Download the updated target profile as a new XML file.
- **No Installation Required:** 100% client-side, works in any modern browser. No dependencies, no server, no data leaves your computer.
- **Emojis for Clarity:** Uses emoji icons for a modern, intuitive interface.

---

## Usage

1. **Open the App:**  
   Download and open `JG_ActionCopier.html` in your web browser.

2. **Load Profiles:**  
   - Select one or more source XML profiles.
   - Select a single target XML profile.

3. **Browse and Search:**  
   - Explore the source library and target destinations.
   - Use the search box to quickly find actions.

4. **Copy Actions:**  
   - Select a source action and a target destination.
   - Click "Preview Copy" to review the operation.
   - Confirm or cancel in the preview modal.

5. **Save Changes:**  
   - When ready, enter an output filename and click "Save Modified Profile" to download your updated XML.

---

## Advanced Functionality

- **XML Validation:** The app validates your XML before and after each operation, ensuring your profiles remain error-free.
- **Tooltip Previews:** Hover over any item in the tree to see a tooltip with the relevant XML snippet.
- **Operation Log:** Review a detailed log of all copy/replace actions performed in your session.
- **Search & Filter:** Find actions by any attribute (`name`, `description`, `label`), case-insensitive and matching anywhere in the text.

---

## Requirements

- Any modern web browser (Chrome, Edge, Firefox, Safari)
- Joystick Gremlin XML profiles
- Windows 11 (latest version/patches) and Microsoft Edge (latest version/patches) recommended for best compatibility

---

## License

MIT License

---

- **Created by Gemini 2.5 Pro.** did most of the work.
- Claude Sonnet 3.7 - Only did the preview and filter by non-empty-actions
- Chat GPT 4.1 - Wrote most of the README.md 
