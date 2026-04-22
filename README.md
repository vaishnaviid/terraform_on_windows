# Terraform Setup & Usage on Windows (with VS Code)
      
## ✅ 1. Install Terraform on Windows
                                
### **Method 1: Using Chocolatey (Recommended)**  
If you have Chocolatey installed:
                              
```powershell
choco install terraform

```
Verify installation:
```powershell
terraform --version
```
Method 2: Manual Installation
1. Download Terraform ZIP from the official website:
https://developer.hashicorp.com/terraform/downloads

2. Extract the ZIP → You will get terraform.exe.

3. Move terraform.exe to a folder, e.g.:
C:\terraform

4. Add the folder to your PATH:

- Search: Edit the system environment variables

- Click Environment Variables

- Under System variables → select Path

- Click Edit → New

- Add: C:\terraform

- Save and exit

Verify version:

``` powershell
terraform --version
```
✅ 2. Install Git (Optional)
``` powershell
winget install --id Git.Git -e --source winget
```
✅ 3. Install Visual Studio Code
Download from:
https://code.visualstudio.com/

✅ 4. Install Required VS Code Extensions
| Extension Name        | Purpose                                    |
|-----------------------|--------------------------------------------|
| HashiCorp Terraform   | Syntax highlighting, linting, IntelliSense |
| Prettier              | Auto-format JSON                           |
| YAML (RedHat)         | YAML validation for CI/CD                  |

To install extensions:
1. Open VS Code
2. Press Ctrl + Shift + X
3. Search each extension
4. Click Install

✅ 5. Create a Terraform Project
Create folder structure:

```
terraform-project/
├── main.tf
├── variables.tf
├── outputs.tf
└── provider.tf
```

🎉 Terraform is Ready on Your Windows + VS Code Setup!
