# visual-studio-code-on-fedora-30
Visual Studio Code is a wonderful editor for coding! If added completely, updates may happen automatically, here is how

# Terminal Commands
<https://duckduckgo.com/?q=fedora+30+adding+visual+studio+code+repository&kp=-2&kn=1&ia=web>
<https://computingforgeeks.com/install-visual-studio-code-on-fedora/>

$ sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc

$ cat <<EOF | sudo tee /etc/yum.repos.d/vscode.repo
[code]
name=Visual Studio Code
baseurl=https://packages.microsoft.com/yumrepos/vscode
enabled=1
gpgcheck=1
gpgkey=https://packages.microsoft.com/keys/microsoft.asc
EOF

$ dnf check-update

$ sudo dnf install code

$ rpm -qi code
Name        : code
Version     : 1.39.2
Release     : 1571154220.el7
Architecture: x86_64
Install Date: Wed 06 Nov 2019 01:54:42 PM PST
Group       : Development/Tools
Size        : 241045294
License     : Multiple, see https://code.visualstudio.com/license
Signature   : RSA/SHA256, Tue 15 Oct 2019 02:15:49 PM PDT, Key ID eb3e94adbe1229cf
Source RPM  : code-1.39.2-1571154220.el7.src.rpm
Build Date  : Tue 15 Oct 2019 08:43:53 AM PDT
Build Host  : 1d00869ccb6d
Relocations : (not relocatable)
Packager    : Visual Studio Code Team <vscode-linux@microsoft.com>
Vendor      : Microsoft Corporation
URL         : https://code.visualstudio.com/
Summary     : Code editing. Redefined.
Description :
Visual Studio Code is a new choice of tool that combines the simplicity of a code editor with what developers need for the core edit-build-debug cycle. See https://code.visualstudio.com/docs/setup/linux for installation instructions and FAQ.
