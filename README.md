# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.

## DESIGN STEPS:
### Step 1:
Use tools like Autopsy or Sleuth Kit (blkls, icat) to identify and analyze unallocated space.

### Step 2:
Extract data from unallocated space and examine for hidden or deleted content.

### Step 3:
Document and interpret findings as part of the digital investigation process.

## PROGRAM:
Data Extraction and Investigation Tool Usage
```bash
lsblk
```

```bash
sudo dd if=/dev/sda of=/home/kali/disk.img bs=512
```

```bash
mmls ~/disk.img  (sleuth-kit)
sudo fdisk -l ~/disk.img (GNU)

```
#### File may be in a different directory
```
find ~ -name "disk.img" 2>/dev/null

```
```bash
sudo ls -lh /home/kali/disk.img
```
```bash
strings disk.img | less

```


## OUTPUT:
![image](https://github.com/user-attachments/assets/2f6331f7-3f07-4d7c-9371-b4fdabc9f0f7)

![image](https://github.com/user-attachments/assets/106da298-4228-4516-83d3-45f49fb7dd31)

![image](https://github.com/user-attachments/assets/e2824d26-49af-46f1-805c-32fea835b30a)

![image](https://github.com/user-attachments/assets/d5a1771e-b15a-4501-a6d7-d83f9e2fa562)


![image](https://github.com/user-attachments/assets/cf579776-ca7a-4d06-843b-70970ce8a94a)

![image](https://github.com/user-attachments/assets/48903914-d68b-41ac-8cfc-a6d9259cab53)

![image](https://github.com/user-attachments/assets/0b09fa21-7b0d-4fef-a627-e2104a76d1e3)



## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.
