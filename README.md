# Quick Guide: Spin Up VMs with Vagrant in VMware

Make sure you already have **VMware installed** before proceeding.

---

## 1. Vagrant Installation for VMware

1. Go to the Vagrant website and download the installer:  
   [https://developer.hashicorp.com/vagrant](https://developer.hashicorp.com/vagrant)  
   Install Vagrant following the instructions on the website.

2. To make Vagrant work with VMware, you need two additional steps:

   - **Download and install VMware utilities**:  
     [https://developer.hashicorp.com/vagrant/docs/providers/vmware/vagrant-vmware-utility](https://developer.hashicorp.com/vagrant/docs/providers/vmware/vagrant-vmware-utility)  

   - **Install the VMware plugin** (for Windows):  
     ```bash
     vagrant.exe plugin install vagrant-vmware-desktop
     ```

3. **Restart your system** to apply changes.

---

## 2. Create VM

1. Clone this repository:  
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Run Vagrantfile
   ```bash
   vagrant.exe up
   ```

   ---

## 3. Make the VM Show up in VMware
1. Open VMware and go to File → Scan for Virtual Machines.
2. Navigate to the .vagrant.d directory in your home folder: $HOME/.vagrant.d
3. Wait untill it finds your VM
4. Click finish

---

## 4. Access Your Provisioned Kali VM
