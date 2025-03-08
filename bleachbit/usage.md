To clean all temporary and cache data on Windows using BleachBit via the command line, you can use the following steps:

1. Open the Command Prompt with administrative privileges.
2. Navigate to the directory where BleachBit is installed. For example:
   ```cmd
   cd "C:\Program Files (x86)\BleachBit"
   ```
3. Use the `bleachbit_console.exe` command with the appropriate options. For cleaning all temporary and cache data, you can use:
   ```cmd
   bleachbit_console.exe --clean system.tmp system.cache
   ```

You can also list all available cleaning options with:
```cmd
bleachbit_console.exe --list
```

Make sure to preview the changes before cleaning to avoid accidental deletion of important files:
```cmd
bleachbit_console.exe --preview system.tmp system.cache
```

---

Using BleachBit effectively to clean your Windows system requires caution, as overly aggressive cleaning could lead to the unintended removal of essential files. Below are some important and useful BleachBit commands for keeping your system clean without breaking it. These are safe options for regular maintenance:

### General and Safe Cleaning Commands
1. **Clean Temporary Files and Cache:**
   ```cmd
   bleachbit_console.exe --clean system.tmp system.cache
   ```

2. **Clear Browser Data (e.g., Cookies, History, Cache):**
   Replace `firefox` or `chrome` with your browser of choice:
   ```cmd
   bleachbit_console.exe --clean firefox.cache firefox.cookies firefox.history
   bleachbit_console.exe --clean chrome.cache chrome.cookies chrome.history
   ```

3. **Clear Windows System Logs and Debug Files:**
   ```cmd
   bleachbit_console.exe --clean system.logs system.debug
   ```

4. **Clean Thumbnail Cache:**
   ```cmd
   bleachbit_console.exe --clean system.thumbnails
   ```

5. **Wipe Free Disk Space (to prevent recovery of deleted files):**
   ```cmd
   bleachbit_console.exe --clean system.free_disk_space
   ```

### Listing Available Options
To see all available options for cleaning:
```cmd
bleachbit_console.exe --list
```

### Preview Before Cleaning
It’s essential to preview the changes first:
```cmd
bleachbit_console.exe --preview system.*
```

### Important Tips to Avoid Issues
- **Always Preview:** Use the `--preview` flag before executing commands.
- **Avoid Cleaning Essential System Files:** Do not select options like "registry" unless you're experienced and understand the consequences.
- **Backup Your Data:** It’s a good idea to back up important files before running any cleaning process.

If you're looking for a fully clean but safe experience, start with the general commands above and explore additional cleaning options carefully using the `--list` command. Let me know if you need a detailed guide on customizing your cleanup!
