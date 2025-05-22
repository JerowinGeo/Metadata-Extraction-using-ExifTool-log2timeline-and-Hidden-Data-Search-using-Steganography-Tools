# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
### Name : Jerowin Geo J A
### Reg.No : 212223100016
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
### A. Using ExifTool – for file metadata
#### Install:
sudo apt update
sudo apt install exiftool -y
#### Extract metadata from a file:
exiftool image.jpg
#### Batch process a folder:
exiftool -r /path/to/folder
#### Useful flags:
```
- G: Show metadata group
```
```
- time:all: Show only timestamps
```
```
- GPSLatitude -GPSLongitude: Extract GPS data
````
![image](https://github.com/user-attachments/assets/bee2fe7f-4e87-4d9f-858e-47767f321ff2)


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
![image](https://github.com/user-attachments/assets/b686c4cd-b4f9-45f5-9984-8dfbc6e256f3)

## -Extract hidden data:
```
steghide extract -sf hidden.jpg
```

![image](https://github.com/user-attachments/assets/ab37f716-86a8-43cf-a453-44fb08c55db5)


## Using binwalk – for file analysis
```
sudo apt install binwalk -y
binwalk suspicious.jpg
```
```
binwalk /home/kali/Downloads/wallpaper.jpg
```
![image](https://github.com/user-attachments/assets/02c84426-074b-4259-8f48-1d599da13374)


## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.
