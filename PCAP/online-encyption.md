<img width="589" height="209" alt="image" src="https://github.com/user-attachments/assets/fdcd18fc-9082-452e-8fb3-9513fb8f421a" />Category : Network Forensics  
Level : Easy  
Challenge Link : https://app.cyber-edu.co/challenges/55c7c4e0-7f21-11ea-9429-9367630f4e1e?tenant=cyberedu<br>

<img width="238" height="157" alt="image" src="https://github.com/user-attachments/assets/17b78ae1-87d5-47ef-bed1-e08dd2f6adcd" />
<br>
Since this is online-encryption, I need to find something related to Cryptography( SHA, AES, WAP,..) 
<br>
<img width="599" height="118" alt="image" src="https://github.com/user-attachments/assets/75fe4520-965b-4d15-91a7-14c5705a755d" />
<br>
From line number 11017 to 11535, I found the AES encryption key and item
<br>
<img width="259" height="59" alt="image" src="https://github.com/user-attachments/assets/1e23bd53-6ebe-4bf5-b0ec-73ecd0350556" />
<br>
UlBGUHtxcTU0NX  
NvczEyc3E2MDhx  
bm44cDIwMXM1MH  
M5NXA4NTIwb3Jw  
OXM3NDRuMzU3M2  
8xcXAwb3A1M3By  
MDE5NzI2fQ==  
<br>
That looks like Base64. Decode it on Cyberchef.<br>
RPFP{qq545sos12sq608qnn8p201s50s95p8520orp9s744n3573o1qp0op53pr019726}<br>
The flag format is ECSC so I need to use caesar cipher.<br>
<img width="589" height="209" alt="image" src="https://github.com/user-attachments/assets/54045ae1-94f6-4968-9f8d-87ae87062d86" />
<br>
ECSC{dd545fbf12fd608daa8c201f50f95c8520bec9f744a3573b1dc0bc53ce019726}<br>
