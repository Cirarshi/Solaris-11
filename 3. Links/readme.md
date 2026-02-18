# Links in Solaris (Soft Links and Hard Links)

This section explains **file linking in Solaris**, covering both **soft (symbolic) links** and **hard links**.  
Links allow multiple references to files, helping with flexibility, organization, and efficient filesystem usage.

---

## Soft Link (Symbolic Link)

A **soft link** is a special file that points to another file or directory by its **path name**.

- Acts like a shortcut
- Can link to directories
- Breaks if the original file is deleted or moved

### Create a Soft Link

ln -s <original_file> <soft_link>

**Example:**
```sh
ln -s /var/log/syslog syslog_link
```

## Hard Link

A **hard link** is another name for the same file, pointing directly to the file’s inode.

- Both names share the same data on disk
- File remains accessible as long as one hard link exists
- Cannot be created for directories

### Create a Hard Link

ln original_file hard_link

**Example:**
```sh
ln data.txt data_backup.txt
```

### Unlinking a link

unlink <link name>

---

| Feature | Soft Link (Symbolic Link) | Hard Link |
|--------|---------------------------|-----------|
| Points to | File path | Inode |
| Can link directories | Yes | No |
| Works across filesystems | Yes | No |
| Breaks if original file is deleted | Yes | No |
| Inode number | Different | Same |
| File size | Small (stores path reference) | Same as original |
