# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
### Name : SANJAY M S 
### Reg.No : 212223040183
## AIM:
To extract metadata, perform timeline analysis, and search for hidden data using forensic tools like ExifTool, log2timeline, and steganography detection tools.

## DESIGN STEPS:
### Step 1:
Use exiftool to extract metadata from files such as images, documents, and videos.

### Step 2:
Use log2timeline and plaso to create and analyze event timelines from system logs and file metadata.

### Step 3:
Apply steganography detection tools like steghide, zsteg, or binwalk to uncover hidden data in media files.

## PROGRAM:
Metadata and Timeline Forensics, Steganography Analysis Steps

## OUTPUT:
### ✅ A. Using ExifTool – for file metadata
#### 📦 Install:
sudo apt update
sudo apt install exiftool -y
#### 📂 Extract metadata from a file:
exiftool image.jpg
#### 📁 Batch process a folder:
exiftool -r /path/to/folder
#### 📌 Useful flags:
```
- G: Show metadata group
```
```
- time:all: Show only timestamps
```
```
- GPSLatitude -GPSLongitude: Extract GPS data
````
![435680836-861dc1d1-4932-460d-9261-2e3295ee9f42](https://github.com/user-attachments/assets/8192aafb-f53b-4b92-ab1f-09b2f572028a)


### install log2timeline

```
sudo apt install plaso -y
```
```
sudo apt install steghide -y
```

## -Embed data

```
steghide embed -cf /home/kali/Downloads/wallpaper.jpg -ef /home/kali/Downloads/secret.txt
```
![image](https://github.com/user-attachments/assets/4791e632-ca36-4e1f-9149-5633f480d1fc)

## -Extract hidden data:
```
steghide extract -sf hidden.jpg
```

![435686036-85520110-9150-417a-b6a9-28e559100cf7](https://github.com/user-attachments/assets/014c88ff-4f61-40d3-b9f3-1ffef40fc018)


## Using binwalk – for file analysis
```
sudo apt install binwalk -y
binwalk suspicious.jpg
```
```
binwalk /home/kali/Downloads/wallpaper.jpg
```
![435687161-b26be271-0680-491f-8868-1216de6fd7eb](https://github.com/user-attachments/assets/2298b20a-6f79-4231-99e6-b48f7860732c)


## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.
