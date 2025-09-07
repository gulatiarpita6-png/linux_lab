# FIRST LAB

---

### ✅ Contents of the Markdown file:

````markdown
# Linux File Commands Cheat Sheet
````
---
``
### 1 `mkdir` – Make Directory

Creates a new folder.

```bash
mkdir new_folder
```

### 2. `rm` – Remove a File or Directory

- **Usage:**
  ```bash
  rm filename
````
````
* **Examples:**

  ```bash
  rm my_file.txt         # Delete a file
  rm -r my_folder/       # Delete a folder and its contents
  rm -f important.txt    # Force delete without prompt
  ```

---

## 3. `cp` – Copy Files or Directories

* **Usage:**

  ```bash
  cp source destination
  ```

* **Examples:**

  ```bash
  cp file.txt backup.txt           # Copy a file
  cp file.txt /home/user/docs/     # Copy file to another folder
  cp -r folder1/ folder2/          # Copy directories recursively
  ```

---

## 4. `touch` – Create an Empty File

* **Usage:**

  ```bash
  touch filename
  ```

* **Examples:**

  ```bash
  touch newfile.txt           # Create a new empty file
  touch a.txt b.txt c.txt     # Create multiple files at once
  ```

---

## 5. `mv` – Move (or Rename) a File

* **Usage:**

  ```bash
  mv source destination
  ```

### 🧪 Example: Move a File

```bash
# Step 1: Create a file
touch file1.txt

# Step 2: Create a folder
mkdir my_project

# Step 3: Move file1.txt into my_project/
mv file1.txt my_project/
```

![alt text](image.png)

### 🔐 `chmod` – Change File Permissions

Basic syntax:

```bash
chmod [permissions] file
```

#### Common Usage:

```bash
chmod 755 script.sh     # Owner: read/write/execute; others: read/execute
chmod +x file.sh        # Add execute permission
chmod -x file.sh        # Remove execute permission
```

### 🔢 What Do Numbers Mean?

| Number | Permission             |
| ------ | ---------------------- |
| 7      | read + write + execute |
| 6      | read + write           |
| 5      | read + execute         |
| 4      | read only              |
| 0      | no permission          |

Example:

```bash
chmod 644 file.txt
# Owner: read/write, Group: read, Others: read
```

---

### 👑 `chown` – Change File Owner

```bash
sudo chown user:group file
```

Example:

```bash
sudo chown alice:alice myfile.txt
```

---

<img width="771" height="517" alt="image-7" src="https://github.com/user-attachments/assets/c6485736-bbaf-4385-82c3-c2f61482bf2a" />
