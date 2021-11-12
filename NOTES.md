# NOTES

---

## For SonarQube
compose kaldırılmadan önce bazı konfigürasyonlar yapılmalı. linuxta problem yaşadım

vi /etc/sysctl.conf

vm.max_map_count=262144
fs.file-max=65536

sysctl -p

vi /etc/security/limits.d/99-sonarqube.conf

root   -   nofile   65536
root   -   nproc    7610

reboot

---
