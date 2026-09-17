Category : Forensics  
Level : Easy  

<img width="471" height="331" alt="image" src="https://github.com/user-attachments/assets/fb8b78f8-000b-4e31-b9a5-0aa6078facf7" />  

That BBBBBB... is probably in the ascii of the file.<br>
Search with this command => 
strings chall.jpg | grep BBBBBBBBBB<br>

<img width="325" height="381" alt="image" src="https://github.com/user-attachments/assets/dac9c050-d060-4f80-a87d-7129c14274f6" />  

Remove the BBB... text, I use this command => sed -i 's/BBBBBBBBBB//g' chall.jpg<br>
Vola!! I correctly created the flag image.<br>
<img width="621" height="415" alt="image" src="https://github.com/user-attachments/assets/af18be30-65f1-43eb-b0c5-7b7187340583" /><br>
TFCCTF{the_fl4g_1s_th3_w4y}<br><br>
The main command works like this :<br>
sed = stream editor<br>
-i = modify the original file directly<br>
s/old/new/g = substitute old with new everywhere<br>
here, old is BBBBBBBBBB<br>
new is empty, so it deletes it<br>
g = replace every occurrence on each processed line
