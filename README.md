## Download Microsoft Remote Desktop

Before connecting to your devices or applications from a Windows machine, ensure the following prerequisites are met:

A stable internet connection.
A device running one of the supported Windows editions listed below:

Windows 11
Windows 10
Windows Server 2022
Windows Server 2019
Windows Server 2016

* .NET Framework 4.6.2 or later. You might need to install this on Windows Server 2016 or certain Windows 10 editions. To obtain the latest version, see .NET Framework download.

Follow these steps to install the Remote Desktop client on Windows using the MSI installer. For enterprise deployment, you can use `msiexec` from the command line to install the MSI package.

1. Download the Remote Desktop client installer, selecting the version suitable for your device:

* [Windows 64-bit](*) *(most common)*
* [Windows 32-bit](*)
* [Windows ARM64](*)

2. Run the installer by double-clicking the downloaded file.

3. On the welcome screen, choose **Next**.

4. To accept the license agreement, tick **I accept the terms in the License Agreement**, then select **Next**.

5. Choose the Installation Scope:

* **Install just for you**: Installs Remote Desktop in a per-user folder for your account only. No administrator privileges required.
* **Install for all users of this machine**: Installs in a per-machine folder, available to all users. Local Administrator privileges are required.

6. Click **Install**.

7. After installation completes, select **Finish**.

8. If **Launch Remote Desktop when setup exits** is checked, the client will open automatically. Otherwise, launch Remote Desktop from the Start menu.

> **Important**

> If both the Remote Desktop client (MSI) and the Azure Virtual Desktop app from Microsoft Store are installed, you may see a message starting **A version of this application called Azure Virtual Desktop was installed from the Microsoft Store**. Both applications are supported, but using the same resources across both apps may cause confusion. We recommend using only one app version at a time.

## Subscribe to a workspace

A workspace consolidates all desktops and applications assigned by your admin. To view these in the Remote Desktop client, subscribe to the workspace as follows:

1. Open the **Remote Desktop** app.

2. When subscribing for the first time, on the **Let's get started** screen, select **Subscribe** or **Subscribe with URL**.

* If **Subscribe** is chosen, sign in with your user account, for example `user@contoso.com`. After a few seconds, your desktops and applications should appear.

If the message **No workspace is associated with this email address** appears, your admin may not have configured email discovery, or you may be in a non-Azure cloud (e.g., Azure for US Government). In this case, use **Subscribe with URL**.

* If **Subscribe with URL** is selected, enter the workspace URL in the **Email or Workspace URL** field. After a few seconds, the message **We found Workspaces at the following URLs** should appear.

3. Select **Next**.

4. Sign in when prompted. The workspace will then display the desktops and applications made available by your admin.

Once subscribed, the workspace content updates automatically regularly and whenever the client starts. Resources may be added, changed, or removed by the admin.

## Connect to your desktops and applications

To launch your desktops and apps:

1. Open the **Remote Desktop** client.

2. Double-click a desktop or app icon to start a session to Azure Virtual Desktop. Depending on your admin’s configuration, you may be prompted to re-enter your account password.

## Insider releases

To assist in testing new builds before public release, download Insider releases. Organizations can use these versions to validate updates for their users prior to general availability.
