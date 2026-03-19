# MSIX-Application-Packaging
MSIX Conversion &amp; Modernization Project
# MSIX Application Packaging Project

## 📌 Overview
This project demonstrates the conversion of 5 legacy Windows applications into modern MSIX format for better security, clean installation, and easy deployment.

---

## 🛠️ Applications Used
- 7-Zip  
- WinSCP  
- GIMP  
- Inkscape  
- Notepad++  

---

## ⚙️ Tools & Technologies
- MSIX Packaging Tool  
- Process Monitor  
- Windows SDK (SignTool, MakeAppx)  
- PowerShell  
- Package Support Framework (PSF)  

---

## 🔄 Project Workflow
1. Application Discovery  
2. Environment Setup (Windows VM)  
3. MSIX Packaging  
4. PSF Implementation  
5. Code Signing  
6. Testing & Validation  
7. Deployment  
---

## 🚀 Key Features
- Clean Install & Uninstall  
- No Admin Rights Required  
- Secure Sandbox Execution  
- Easy Enterprise Deployment  

---

## ⚠️ Limitations
- Driver-based apps not supported  
- Requires code signing  
- Complex apps may need PSF  

---
## 📂 Project Files
- 📊 PPT: Project Presentation  
- 📄 DOC: Detailed Documentation  
- 🖼️ Screenshots  
---
## 📌 Conclusion
MSIX provides a modern, secure, and efficient way to deploy and manage applications in enterprise environments.


## 💻 PowerShell Deployment

Below is a sample PowerShell command used to install MSIX packages:

```powershell
Add-AppxPackage -Path "C:\Packaging\Output\YourApp.msix"
$apps = @(
    "C:\Packaging\Output\7zip.msix",
    "C:\Packaging\Output\WinSCP.msix",
    "C:\Packaging\Output\GIMP.msix"
)

foreach ($app in $apps) {
    Add-AppxPackage -Path $app
}

 🔗 Author
**Anshika Kumari**
