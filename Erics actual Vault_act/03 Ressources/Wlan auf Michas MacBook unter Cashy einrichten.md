---
training:
tags:
  - pkm
type:
  - "[[evergreen]]"
status: new
project:
  - "[[MacBook von Micha auf Cashy umstellen]]"
area:
context:
---


# Wlan auf Michas MacBook unter Cashy einrichten
## 2026-02-11 19:18
___
# Abstract
```bash
# 1. modprobe.d (Entropy + Stabil)
echo 'options brcmfmac feature_disable=0x82000 roamoff=1' | sudo tee /etc/modprobe.d/brcmfmac.conf
```
```bash
# 2. Entropy-Daemon (WPA3-Handshake)
sudo pacman -S haveged
sudo systemctl enable --now haveged
```
```bash
# 3. Initramfs + Limine
sudo mkinitcpio -P
sudo limine-update
reboot
```


# Analysis 
- That is interesting …
	- 
- It reminds me of…
	- 
- It is similar to ... because…
	- 
- It is different to ... because…
	- 
- It is important because…
	- 


---
## Reference:
**ÜBERGEORDNETE NOTIZ** 

**LITERATURNOTIZ**

**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]

