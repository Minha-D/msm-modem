# msm-modem
To setup up Qualcomm QMI modem on Linux distros
This script "setup-msm-modem.sh" will run at boot time.
Thanks to systemd service "setup-msm-modem.service".But this service needs to run before rmtfs(Qualcomm Remote Filesystem Service Implementation).
Now this repo would just support Arch Linux. In future I would make it avilable for other distros like debian,fedora,etc.
# Dependencie
msm-modem requres rmtfs to load firmware in qcom qmi modems.
PKGBUILD will automatically install rmtfs.So make sure that it is installed.
# HOW TO INSTALL
1. Clone this repo.
2. Open terminal.
3. cd msm-modem.
4. "makepkg -si" to install.
5. Make sure to enable setup-msm-modem.service using "sudo systemctl enable setup-msm-modem".
