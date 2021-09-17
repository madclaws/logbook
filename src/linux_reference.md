> Captain's log, Stardate **2122.261.13**

# Linux commands reference

1. **List all open ports**

    `sudo lsof -i -P -n | grep LISTEN`
2. **Info about the process running on a port**

    `lsof -i :<PORT>`

3. **Location of the running process**
    
    `lsof -p <PID> | grep cwd`

4. **Killing a process**

    `kill <PID>`

5. **Copying a folder**

    ``` cp -avr /tmp/conf/ /tmp/backup/ ```

6. **Removing files older than X days**

    ``` find <path>/*.log -mtime +X -exec rm {} \;  ```

-------------------