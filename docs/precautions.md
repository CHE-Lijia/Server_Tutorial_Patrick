# Precautions & Security

Welcome to the lab's shared server environment. Because this is a multi-user system, following these guidelines is **mandatory** to ensure data integrity, system stability, and fair access for all lab members.

---

## 1. Data Safety & Storage
*   **Do Not Delete Others' Data:** Never modify, move, or delete files or directories that do not belong to you without explicit permission from the owner.
*   **Restrict File Permissions:** To protect your research data, ensure that your personal directories and files are not world-writable. **Never** use `chmod 777` on your folders. Use `chmod 700` (read/write/execute only for you) or `chmod 755` (read/execute for others, write only for you) to ensure that other users cannot accidentally modify or delete your work.
*   **Storage Locations:** 
    *   Use your home directory (`/home/username`) for personal configuration files and scripts.
    *   Use the designated data partition (`/hdd1/username`) for large datasets and heavy processing. 
    *   **Avoid** running heavy I/O operations directly on the system root partition.

*   **Backups:** The server is not a permanent storage solution. Always keep a local copy of your critical research data. If you are working on long-term projects, ensure you have a backup strategy (e.g., external hard drives or cloud storage or Github).

## 2. Resource Management
*   **Monitor Resource Usage:** Before starting a heavy job, check the current load using `htop` or `nvidia-smi` (if using GPUs). Do not overload the server if others are already running intensive tasks.
*   **Naming Conventions:** Please name your directories and files clearly. Avoid using spaces or special characters in filenames, as they can cause issues with scripts and pipelines.

## 3. Account Security
*   **No Account Sharing:** Your account is for your personal use only. Do not share your password or SSH keys with anyone else.

## 4. Software and data access
*   **Installation:** If you need to install software, check whether it can be installed in conda environment or only for user. Be careful about the softwares requiring root/sudo access. Do not attempt to modify system configuration files yourself.

---
