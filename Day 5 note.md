### Notes on "Advanced Linux User!" (Day5_LinuxRUN.md)

#### Last Time Topics
- Further on User management
- Linux File Ownership + Permissions

#### Today's Class Topics
- Software Installation
- Script Installation
- Package Installation Common errors
- Some advanced user commands

---

#### Advanced User Commands
- **Change Password**: `sudo passwd username`
- **Change User ID**: `sudo usermod -u new_id username`
- **Delete User**: `sudo userdel -r username`
- **Change Users on Terminal**: `su - username`

---

#### Sudoers File
- **Purpose**: Allocate system rights to users.
  
- **Access**: `sudo visudo`
  
- **Add User**: After editing, a user can use `sudo` commands.

---

#### Linux File Permission
- **Components**:
  - Owner
  - Permissions
  - Date
  - Size
  - Filename
  
- **Ownership**:
  - User
  - Group
  
- **Change Ownership**: `chown user:group filename`

---

#### Permission Types
- **Read (r)**
- **Write (w)**
- **Execute (x)**

---

#### CHMOD Command
- **Symbolic Parameters**:
  - `chmod a+x filename`: Add execute permission for all.
  - `chmod u+x filename`: Add execute permission for user.
  - `chmod g+x filename`: Add execute permission for group.
  - `chmod o+x filename`: Add execute permission for others.
  
- **Numeric Parameters**:
  - `chmod 621 filename`: 6 for user, 2 for group, 1 for others (6=rw).
  - `chmod 777 filename`: 7 for user, group, and others (7=rwx).

---

#### Special File Permissions
- **SUID (s)**: `4000`
- **SGID (S)**: `2000`
- **Sticky Bit (t)**: `1000`

---

#### Package Installation on Linux
- **Package Managers**: apt, pacman, pkg, etc.
  
- **APT**: Debian package manager.
  
- **Commands**:
  - `sudo apt update`
  - `sudo apt search <softwarename>`
  - `sudo apt install <softwarename>`
  - `sudo apt remove <softwarename>`
  - `sudo apt upgrade`
  - `sudo apt purge <softwarename>`

---

#### Package Dependencies
- **Modules**: Programs that a software depends on.

---

#### DPKG (Debian Package Manager)
- **Syntax**:
  - `sudo dpkg -i <packagename>`
  - `sudo dpkg -r <packagename>`
  - `sudo dpkg -P <packagename>`

---

#### Assignment
1. Update your system repository.
2. Search for package called ‘cmatrix’.
3. Install ‘cmatrix’.
4. Remove ‘cmatrix’.
5. Create file called “Perm.txt” and give permissions.
6. Answer permission-related questions.
7. Create users and modify their permissions.
8. Install and practice with some programs.

---

**End of Class**