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
