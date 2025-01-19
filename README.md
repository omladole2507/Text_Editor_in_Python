# Text Editor Application ✍️

## Overview
This application is a feature-rich text editor built using Python and the Tkinter library. It includes essential text editing features such as creating, opening, saving, undoing, redoing, and more. Additionally, it incorporates an undo-redo stack mechanism for efficient editing.

---

## Features 🌟

### File Operations 📂
1. **New File:**
   - Create a new blank document.
   - Prompts the user to save changes if the current document is unsaved.

2. **Open File:**
   - Open an existing file from your system.
   - Supported file types:
     - All Files (`*.*`)
     - Python Files (`*.py`)
     - Text Documents (`*.txt`)

3. **Save File:** 💾
   - Save changes to the currently opened file.
   - Prompts the user to save to a new file if none is opened.

4. **Save As:** 📝
   - Save the current content to a new file.

5. **Exit:** ❌
   - Exit the application, with a prompt to save unsaved changes.

### Edit Operations ✂️
1. **Undo:** ↩️ Reverse the last action.
2. **Redo:** ↪️ Reapply the last undone action.
3. **Cut:** ✂️ Remove selected text and copy it to the clipboard.
4. **Copy:** 📋 Copy selected text to the clipboard.
5. **Paste:** 📥 Insert clipboard content at the cursor position.

### View Options 👁️
1. **Change Mode:** 🌗
   - Switch between light and dark modes for better readability.

### Help 💡
1. **About:** ℹ️
   - Displays details about the application from a file named `About.txt`.

---

## How to Run 🚀
1. Ensure you have Python installed on your system.
2. Install the `tkinter` module (usually included in standard Python installations).
3. Save the code in three separate files:
   - `Window.py` for the main application logic.
   - `Stack.py` for the undo/redo stack functionality.
   - `main.py` for initializing and running the application.

4. Run the `main.py` file using the command:
   ```bash
   python main.py
   ```

---

## Dependencies 📦
- Python 3.x
- Tkinter (standard Python library)

---

## File Structure 📁
1. **`main.py`:** Entry point of the application.
2. **`Window.py`:** Contains the `Window` class for managing the text editor functionality.
3. **`Stack.py`:** Implements the `Stack` class for undo/redo operations.
4. **`About.txt`:** Contains the "About" information displayed in the application.

---

## Keyboard Shortcuts ⌨️
- **Ctrl + N:** 🆕 New File
- **Ctrl + O:** 📂 Open File
- **Ctrl + S:** 💾 Save File
- **Ctrl + D:** ❌ Exit Application
- **Ctrl + Z:** ↩️ Undo
- **Ctrl + Shift + Z:** ↪️ Redo
- **Ctrl + X:** ✂️ Cut
- **Ctrl + C:** 📋 Copy
- **Ctrl + V:** 📥 Paste

---

## Additional Notes 📝
1. **Stacks for Undo/Redo:**
   - Undo and Redo operations are managed by `Stack` objects.
   - The `UStack` (Undo Stack) and `RStack` (Redo Stack) ensure efficient editing without data loss.

2. **Dark Mode:** 🌙
   - A user-friendly night mode for comfortable editing in low-light environments.

3. **About File:** ℹ️
   - Ensure the `About.txt` file is available in the working directory to view the "About" section.

---

## Known Issues ⚠️
- If clipboard access fails during paste, ensure the content is copied correctly.
- Large files might cause slight delays during undo/redo operations.

---

## License 📝
This project is open-source and free to use. Feel free to modify and distribute the application as needed.

