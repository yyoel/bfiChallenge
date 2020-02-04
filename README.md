# Prerequisites

1. Cloud Provider Account (the step bellow will be using GCP)
    - Create VM
    - Add local SSH key to VM

2. Editor & Remote SSH (VSCode)
    - SSH to VM
    - Install SDK Man
    - Intall Java from SDK Man
    - Install Maven from SDK Man
    - Run BFI_API
    - Run BFI_Engine1
    - Run BFI_Engine2

## Step by step

1. Go to **Compute Engine** and **Create Instance**

2. Modify the configuration for the vm
    - **Region**
        - asia-southeast1 (Singapore)
    - **Machine configuration**
        - General-purpose
            - E2 Series
            - e2-standard-2 (2 vCPU, 8 GB memory)
    - **Boot disk**
        - Public images
            - OS: Ubuntu
            - Ver: Ubuntu 16.04 LTS
    - **Firewall**
        - Allow both traffics
    - **Security**
        - SSH Keys
            - Insert your public ssh key to the VM (e.g : id_rsa.**pub**)
    - **Disks**
        - Additional disks
            - Add new disk and click **Done**

3. Click **Create** if you done with the configuration

4. Open VSCode, (and make user you have SSH Remote Extention installed first)

5. Open remote host window
![alt](./images/remote_host_icon.png)
    and then **Remote-SSH: Connect to Host...**

6. 