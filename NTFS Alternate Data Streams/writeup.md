Category : Forensics  
Level : Easy
<br>
<img width="475" height="211" alt="image" src="https://github.com/user-attachments/assets/4e2c6280-cc52-4ab4-b961-fbfd8b13da6d" />
<br>
After extracting the file with winrar, I found this.<br>
<img width="81" height="41" alt="image" src="https://github.com/user-attachments/assets/35db170c-4d09-45df-aa39-2806f516842e" /><br>
This is ADS style, which is a hidden feature of the Windows NTFS file system that allow a single file to store multiple streams of data in addition to its primary visible content.<br>
So I check the file with this powershell command => Get-Item .\Flag.txt.txt -Stream *<br>
Found this flag file.<br>
<img width="399" height="34" alt="image" src="https://github.com/user-attachments/assets/c9e023b0-ff80-4255-87a4-cfc96db2b232" /><br>
By using this command => Get-Content .\Flag.txt.txt -Stream real_flag.txt, I got the flag.<br>
ctf{7ce5567830a2f9f8ce8a7e39856adfe5208242f6bce01ca9af1a230637d65a2d}
