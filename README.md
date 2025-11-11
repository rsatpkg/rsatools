# RSAT (Remote Server Administration Tools)

Download the latest version from Releases page:        
https://github.com/buildoz/RSAT/releases/tag/1.412

RSAT enables IT professionals to remotely manage Windows Server roles and features from a computer running either Windows 10 or Windows 7 Service Pack 1.

## Introduction

RSAT cannot be installed on systems running the Home or Standard editions of Windows. It is only available for Professional and Enterprise editions of the Windows client OS. Unless the download page specifically indicates that RSAT supports a beta, preview, or other prerelease version of Windows, installation and operation require a full (RTM) release of the operating system. Some users have attempted to bypass RSAT MSU limitations manually in order to install it on unsupported editions or builds of Windows, but such actions violate the Windows end-user license agreement.

Installing RSAT is similar to installing Adminpak.msi on client systems running Windows 2000 or Windows XP. However, there's an important difference: in Windows 7, the tools aren’t ready for use immediately after installation. You must manually enable the desired tools from the Control Panel. To do so, go to **Start** > **Control Panel** > **Programs and Features**.

In RSAT packages designed for Windows 10, all tools are automatically enabled after installation. To turn off any tools you don’t need on Windows 7, open **Turn Windows features on or off**.

For those using Windows 7, you’ll need to manually activate the tools corresponding to the roles and features you wish to manage once the RSAT package has been installed.

If you’re managing server roles or features on remote machines running Windows Server 2012 R2, you don’t need to install any extra tools. Simply open the Add Roles and Features Wizard in Windows Server 2012 R2 or newer. On the **Select Features** screen, expand **Remote Server Administration Tools**, choose the tools you need, and complete the wizard to finish the installation.

## RSAT for Windows 10, version 1809 or later versions

> **Note**
> The **Turn Windows features on and off** dialog in Control Panel is not available for use.

Installing RSAT on Windows 10 version 1809 and later is slightly different from previous versions. RSAT is now included as part of the operating system and can be installed via **Optional Features**.
