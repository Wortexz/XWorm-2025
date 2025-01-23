# Malware-as-a-service (MaaS) - Xworm analysis

Let's begin...

XWorm is a commodity malware that is advertised for sale on underground forums and comes with a wide range of features that allows it to siphon sensitive information from infected hosts.    
In addition, XWorm is versatile as it can carry out DDoS (distributed denial of service) attacks, ransomware operations, clipper functions, spread via USB, and deploy additional malware.    
XWorm is capable of dropping several malicious payloads at various points on the system, adding or changing registry entries, and executing commands.    

# Quick malware analysis    
So, we spotted in Lithuania very unique Xworm malware sample which is only detected by 3/69 AV engines.    
Submitted on VirusTotal on:
- First Submission: 2025-01-22 15:23:22 UTC.    
- Low community score is also there, because I have shared this sample with one researcher and he downvoted that sample.
  
![Screenshot 2025-01-23 194638](https://github.com/user-attachments/assets/f46a70ab-42eb-4a68-9dde-c0ae8d3aeb57)    

For exactly two days only 3 detections:    

![Screenshot 2025-01-23 185656](https://github.com/user-attachments/assets/2b6c3b98-8bf8-43bd-b0bc-f9f5c964e804)

# How the malware looks like?

From first sight it looks simple:    

![Screenshot 2025-01-23 190213](https://github.com/user-attachments/assets/2b28ad1c-250a-40b2-92aa-ee4f5d62ea1a)    

__Extracted:__     

![Screenshot 2025-01-23 190326](https://github.com/user-attachments/assets/7faca27a-5771-478e-8e6c-a3e8be790dd6)    

__Note:__ If file extensions are hidden by Windows settings it looks like MP4 file ".com" is not visible.

AND file is signed with VALID Code Signing Certificate    

![Screenshot 2025-01-23 195812](https://github.com/user-attachments/assets/7ce07072-f318-41b0-9a75-27869552c0a2)    


__Launching the file:__    

It's specifically designed to show an error!

![Screenshot 2025-01-23 190412](https://github.com/user-attachments/assets/1d2c0631-1a88-4beb-80ea-3f1513d5ae0c)    

__Whats happening behind the scenes__    

Silently these file are downloaded:    

![Screenshot 2025-01-23 192050](https://github.com/user-attachments/assets/807146fb-7773-4e54-9b60-e3cbc081ced7)

__By simply opening a file, all your saved passwords in Google Chrome, Microsoft Edge, and Firefox can be stolen and probably your PC is remotely controlled__    

# Deeper analysis    


