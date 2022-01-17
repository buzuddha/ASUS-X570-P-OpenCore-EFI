# ASUS-X570-P-OpenCore-EFI  
EFI Folder for OpenCore 0.7.6  

This EFI is partially functional:  

MoBo: ASUS X570-P    
CPU: Ryzen 7 5800X  
GPU: AMD FirePro W7000  
Ethernet: Realtek RTL8111 Integrated (MoBo)  
Bluetooth: Intel TP-link Archer TE50X  
WiFi:  Intel TP-link Archer TE50X   
NVMe: Samsung 980Pro  
RAM: OLOy 4000MHz DDR4  

What works:  
WiFi 
Bluetooth  
Ethernet  
iMessage/Facetime/AppleID  
Audio  
USB2 port personality  
USB3 port personality  
Sleep    
Powerbutton wake from sleep    
~6000 GB/s reads | ~1700 GB/s writes  

What doesn't work:  
Bluetooth wake from sleep  
WiFi

Issues:  

1) Bluetooth wake from sleep works, but then doesn't reconnect the bluetooth mouse nor keyboard. Very weird...    
2) [FIXED]I have tried everything, but can't get the monterey installer to get past this first boot screen    
    https://forum.amd-osx.com/index.php?threads/stuck-on-eb-log-exitbs-start-oc-0-7-3-ryzen-5-1600-rx580-b450m-s2h.2124/  
    https://dortania-github-io.thrrip.space/OpenCore-Install-Guide/troubleshooting/extended/kernel-issues.html#stuck-on-eb-log-exitbs-start   
    Turns out I was using an old OC release. Updated thanks to advice from Aluveitie :) -> installed Monterey, boots up works fine 
