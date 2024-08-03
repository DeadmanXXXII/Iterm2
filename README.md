# Iterm2

Certainly! Here is a detailed list of `iTerm2` commands and configurations. iTerm2 is a popular terminal emulator for macOS, offering advanced features for terminal management.

### **iTerm2 Commands and Configurations**

#### **1. Basic Operations**

- **Open iTerm2:**
  ```bash
  open -a iTerm
  ```
  Launches iTerm2 from the command line.

- **Open a new terminal window:**
  ```bash
  osascript -e 'tell application "iTerm" to create window with default profile'
  ```

- **Open a new tab:**
  ```bash
  osascript -e 'tell application "iTerm" to tell current window to create tab with default profile'
  ```

- **Close the current tab:**
  ```bash
  osascript -e 'tell application "iTerm" to tell current session of current window to quit'
  ```

- **Close the current window:**
  ```bash
  osascript -e 'tell application "iTerm" to close current window'
  ```

#### **2. Session and Profile Management**

- **List profiles:**
  Open iTerm2 Preferences (`Cmd + ,`), go to the Profiles tab to view and manage profiles.

- **Create a new profile:**
  Go to Preferences (`Cmd + ,`) > Profiles > Click the `+` button to add a new profile.

- **Set default profile:**
  Go to Preferences (`Cmd + ,`) > Profiles > Select the profile and click `Default`.

- **Edit profile settings:**
  Go to Preferences (`Cmd + ,`) > Profiles > Select the profile > Edit settings such as colors, fonts, and shell.

#### **3. Advanced Features**

- **Search through terminal output:**
  Press `Cmd + F` to open the search bar and search through the terminal output.

- **Split panes:**
  - **Horizontal split:**
    ```bash
    Cmd + D
    ```
  - **Vertical split:**
    ```bash
    Cmd + Shift + D
    ```

- **Broadcast input to all panes:**
  ```bash
  Cmd + Option + Shift + I
  ```
  Broadcasts the input to all open panes in the current window.

- **Save and load sessions:**
  - **Save current session:**
    Go to `Shell` > `Save Window Arrangement` to save the current session layout.
  - **Load saved session:**
    Go to `Shell` > `Restore Window Arrangement` to load a saved session layout.

#### **4. Customization and Automation**

- **Create custom key bindings:**
  Go to Preferences (`Cmd + ,`) > Keys > Key Bindings > Click the `+` button to add custom key bindings.

- **Set up triggers:**
  - **Create a new trigger:**
    Go to Preferences (`Cmd + ,`) > Profiles > Advanced > Triggers > Click `Edit` and add new triggers based on regular expressions.

- **Configure color schemes:**
  - **Import color schemes:**
    Go to Preferences (`Cmd + ,`) > Profiles > Colors > Click `Color Presets` and select `Import...`.

- **Create a custom command:**
  Go to Preferences (`Cmd + ,`) > Profiles > Command > Run command: and enter the command you wish to run when a new terminal session starts.

#### **5. Integration and Scripting**

- **Run AppleScript from iTerm2:**
  - **Open AppleScript Editor:**
    Use the built-in `Script Editor` app to write and run AppleScripts.
  - **Example script to open a new terminal tab:**
    ```applescript
    tell application "iTerm"
        create tab with default profile
    end tell
    ```

- **Use `tmux` integration:**
  - **Start `tmux` in iTerm2:**
    ```bash
    tmux
    ```
  - **Configure `tmux` settings in iTerm2:**
    Go to Preferences (`Cmd + ,`) > Profiles > Terminal > Integrate with tmux > Enable tmux integration.

- **Set up shell integration:**
  - **Install shell integration:**
    Follow instructions in iTerm2 > Preferences (`Cmd + ,`) > Profiles > Terminal > Install Shell Integration to enable features such as clipboard history and better terminal handling.

#### **6. Troubleshooting and Maintenance**

- **Reset iTerm2 preferences:**
  Go to Preferences (`Cmd + ,`) > General > Preferences > Click `Restore Defaults`.

- **View system logs:**
  Check Console.app or system logs for any iTerm2 related issues.

- **Update iTerm2:**
  - **Check for updates:**
    Go to `iTerm2` > `Check for Updates` to update to the latest version.

### **Summary**

This comprehensive list covers basic and advanced operations, session and profile management, customization, automation, integration, and troubleshooting for iTerm2. With these commands and techniques, you can effectively manage and customize your terminal environment on macOS.
