# HP Elitedesk 800 G1 Mini EFI

<img valign="right" align="right" src="./Images/HP-Elitedesk-800-G1.png" alt="HP Elitedesk 800 G1" width="500">

[![OpenCore](https://img.shields.io/badge/OpenCore-0.9.3-green.svg)](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.9.3)
[![macOS](https://img.shields.io/badge/macOS_Ventura-13.4.1-orange.svg)](https://support.apple.com/en-us/HT213813)

### 💻 Hardware
<details>
<summary><strong>Show</strong></summary>
<br>

| Component                      | Brand/info                                |
|--------------------------------|:-----------------------------------------:|
| **CPU**                        | `Intel® Core i5-4590T 2.0 GHz`|
| **iGPU**                       | `Intel HD Graphics 4600`                 |
</details>

### ⚠️ Not tested
<details>
<summary><strong>Show</strong></summary>
<br>

WiFi card
</details>

## ⚙️ Setup

<details>
<summary><strong>🔧 BIOS Settings</strong></summary>
</br>
Update bios to the latest version and set to default settings then follow
</br>
</br>

|    |                                 |
|----|:-------------------------------:|
| Security -> VTd | `Disabled` |
| Storage -> Storage Options -> SATA Emulation | `AHCI` |
| *Recommended* Power->Thermal->Fan Idle Mode | `lowest` |

</details>

<details>
<summary><strong>🗒 Installation</strong></summary>

|    |                                 |
|----|:-------------------------------:|
| 1. | Install MacOS on a usb (search online many ways to do it)|
| 2. | Place the EFI folder into the EFI partition|
| 3. | Setup SMBIOS [Follow this Part of the Guide](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#using-gensmbios) enter `Macmini8,1 10` in GenSMBIOS|
| 4. | [continue that guide from here](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#serial-number-validity)|
| 5. | After you have replaced the SMBIOS files boot from the USB, Format your ssd, and install MacOS|
| 6. | Once MacOS is installed, download [OpenCore Legacy Patcher (OpenCore-Patcher-GUI.app.zip)](https://github.com/dortania/OpenCore-Legacy-Patcher/releases/tag/0.6.7)|
| 7. | Click "Post install root patch" then click "start root patching" (this will be used to install the gpu drivers)|
| 8. | Select reset nvram from the boot menu (of OC) and boot into MacOS|

</details>

<details>
<summary><strong>🗒 How to boot without the USB</strong></summary>
  
|    |                                 |
|----|:-------------------------------:|
| 1. | [Download OpenCore Configurator](https://mackie100projects.altervista.org/download-opencore-configurator/)|
| 2. | Click Tools (from the top menu)>Mount EFI|
| 3. | Click Mount Partition for both the USB and the system SSD|
| 4. | Copy the files inside the EFI folder on the USB and place them inside the EFI folder on the system SSD |
| 5. | Thats it! everything should work now|
</details>

## ⭐️ Credits
<details>

<br>

[hp_800_g1_mini_hackintosh By asle](https://github.com/asle/hp_800_g1_mini_hackintosh)
</br>
[Donw35 on InsanelyMac](https://www.insanelymac.com/forum/topic/323180-ventura-monterey-big-sur-catalina-mojave-high-sierra-on-hp-800-g1-usdtsff-and-tower-pcs/)
</br>

  
</details>
