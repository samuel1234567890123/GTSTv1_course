### Notes on "Further on Linux" (Day4_MoreLinux.md)

#### Last Time Topics
- awk and sed

#### Topics Covered
1. **Linux File Hierarchy**
2. **Text Editors**
   - VIM
   - NANO
3. **Linux User Management**

---

#### Linux File Hierarchy
- **Difference from Windows**: Linux/UNIX have a distinct file system compared to Windows.
  
- **System Files**:
  - **Windows**: Appear under `local disk C:`
  - **Linux**: Appear under the root directory (`/`)

- **File Structure Overview**:
  - **Root Directory (`/`)**: Starting point for all files and directories, only accessible by the root user.
  - **bin**: Binary executables like `cat`, `ls`, `cp`, `pwd`.
  - **/boot**: Boot loader files like `initrd.img`, `vmlinuz`.
  - **/dev**: Device files such as terminals and USBs.
  - **/etc**: Configuration files and startup/shutdown scripts.
  - **/home**: Home directories for users.
  - **/lib**: Libraries for `/bin` and `/sbin` binaries.
  - **/media**: Mount points for removable media.
  - **/mnt**: Temporarily mounted file systems.
  - **/opt**: Optional application software packages.
  - **/sbin**: Essential system binaries for system maintenance.
  - **/tmp**: Temporary files.
  - **/usr**: User utilities, binaries, libraries, and source-code.

---

#### Text Editors
- **Linux Command Line Text Editors**:
  - VIM
  - Nano
  - Emacs
  - Neovim
  
- **Linux Graphical Text Editors**:
  - Sublime
  - Vscode
  - Gedit
  - Pluma

---

#### VIM
- **History**: Evolution from the line editor `vi` to `VIM` (VI iMproved).
  
- **Features**:
  - Powerful but cryptic.
  - Two modes: Command mode and Input mode.
  
- **Commands**:
  - Save: `:w`
  - Quit: `:q`
  - Save & Quit: `:wq!`
  - Undo: `:undo` or `:u`
  - Execute Bash commands: `:%!yourcommand`

---

#### NANO
- **Description**: User-friendly, free, and open-source text editor.
  
- **Commands**:
  - Save: `Ctrl + S`
  - Undo: `Alt + U`
  - Redo: `Alt + E`
  - Exit: `Ctrl + X`
  - Copy: `Ctrl+shift+C`
  - Cut: `Ctrl+shift+X`
  - Paste: `Ctrl+shift+V`

---

#### Linux User Management
- **User**: Person who uses the computer.
  
- **Groups**: Users belong to groups.
  
- **User Types**:
  - **Root**: ID `0`
  - **Normal User**: ID `1-999`
  
- **SUDO**: Superuser do, used to bypass permission denied.

- **Creating Users**:
  - `useradd`: Simple
  - `adduser`: Detailed

- **User Files**:
  - `/etc/passwd`: User details
  - `/etc/shadow`: User passwords

---

#### Assignment
1. Push your notes to GitHub.
2. Repeat the commands.
3. Stay strong and curious.

---

**End of Class**