# Task 1: Guidelines for VMWare, Ubuntu and Compilers Installation





## Installation of VMWare

## Step 1: Download VMware Software

1. **Visit the Official VMware Website:**
   - Go to the official VMware website at [https://www.vmware.com/](https://www.vmware.com/).

2. **Select the Product:**
   - Choose the VMware product that suits your requirements. Common options include VMware Workstation Player, VMware Workstation Pro, or other VMware solutions.

3. **Download the Installer:**
   - Locate the download section for the selected product and download the installer file.



![image-20240201224616998](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20240201224616998.png)





## Step 2: Run the Installer

1. **Launch the Installer:**
   - Locate the downloaded installer file and double-click to run it.

2. **User Account Control (UAC):**
   - If prompted by User Account Control, click "Yes" to allow the installer to make changes to your device.

## Step 3: Installation Wizard

1. **Welcome Screen:**
   - The installation wizard will open with a welcome screen. Click "Next" to proceed.

2. **End-User License Agreement (EULA):**
   - Read and accept the End-User License Agreement. Click "Next" to continue.

3. **Choose Installation Type:**
   - Select the installation type. For most users, the default settings are suitable. Click "Next" to proceed.

4. **Enhanced Keyboard Driver (Optional):**
   - Decide whether to install the enhanced keyboard driver. Make your selection and click "Next."

## Step 4: License Key (if applicable)

1. **Enter License Key:**
   - If you have a license key, enter it when prompted. Otherwise, choose the option for a free trial or non-commercial use.

## Step 5: Choose Destination Folder

1. **Select Destination Folder:**
   - Choose the folder where you want VMware to be installed. Click "Next" to continue.

## Step 6: Ready to Install

1. **Ready to Install:**
   - Review the installation settings. Click "Install" to start the installation process.

## Step 7: Installation Progress

1. **Installation Progress:**
   - Monitor the progress of the installation. This may take a few minutes.





![image-20240201224737028](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20240201224737028.png)





## Step 8: Complete Installation

1. **Installation Complete:**
   - Once the installation is finished, click "Finish" to exit the installer.

## Step 9: Run VMware

1. **Launch VMware:**
   - Find the VMware application in your Start Menu or Desktop and launch it.

2. **Activate or Log In (if applicable):**
   - Depending on the product, you may need to activate your license or log in with your VMware account.

## Additional Tips:

- **Check for Updates:**
  - After installation, check for updates through the VMware software to ensure you have the latest features and security patches.

- **Read Documentation:**
  - Explore the product documentation for additional features, troubleshooting tips, and best practices.





## Installation of Ubuntu

## Step 1: Download Ubuntu ISO

1. **Visit the Official Ubuntu Website:**
   - Go to [https://ubuntu.com/](https://ubuntu.com/) and navigate to the "Download" section.

2. **Select Ubuntu Version:**
   - Choose the Ubuntu version that suits your requirements (e.g., LTS or the latest stable release).

3. **Download the ISO:**
   - Click on the download link for the selected version to get the Ubuntu ISO file.





![image-20240201224940014](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20240201224940014.png)





## Step 2: Create a New Virtual Machine

1. **Open VMware:**
   - Launch VMware on your Windows system.

2. **Create a New Virtual Machine:**
   - Click on "File" > "New Virtual Machine."

3. **Virtual Machine Configuration:**
   - Choose "Typical" for a standard setup.

4. **Select Installation Disk:**
   - Choose "Installer disc image file (iso)" and browse to the location where you saved the Ubuntu ISO file.

5. **Guest Operating System:**
   - Choose "Linux" as the guest operating system, and for the version, select the appropriate Ubuntu version.

6. **Assign Memory:**
   - Allocate the amount of RAM for the virtual machine. A minimum of 2GB is recommended.

7. **Specify Disk Capacity:**
   - Create a new virtual disk or use an existing one. Allocate sufficient space for your Ubuntu installation.

## Step 3: Begin Ubuntu Installation

1. **Power On the Virtual Machine:**
   - Click "Finish" to complete the setup, then power on the virtual machine.

2. **Select Language:**
   - Choose your preferred language for the Ubuntu installation.

3. **Install Ubuntu:**
   - Select "Install Ubuntu" from the boot menu.

4. **Keyboard Layout:**
   - Choose your keyboard layout.

5. **Updates and Other Software (Optional):**
   - Choose whether to install updates and third-party software during the installation.



![image-20240201225022682](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20240201225022682.png)





## Step 4: Partitioning and Installation

1. **Choose Installation Type:**
   - Select "Erase disk and install Ubuntu" for a straightforward installation.

2. **Select Time Zone:**
   - Set your time zone.

3. **Create User Account:**
   - Enter your name, a username, and a password for your Ubuntu account.

4. **Begin Installation:**
   - Click "Install Now" to start the installation process.

## Step 5: Complete the Installation

1. **System Configuration:**
   - Follow on-screen prompts for system configurations.

2. **Installation Complete:**
   - Once the installation is complete, click "Restart Now."



![image-20240201225109806](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20240201225109806.png)



## Step 6: First Boot into Ubuntu

1. **Remove Installation Medium:**
   - If prompted, remove the installation medium (ISO file).

2. **Login to Ubuntu:**
   - Login using the credentials you created during installation.

3. **Updates and Additional Software:**
   - After logging in, consider updating Ubuntu and installing additional software as needed.

## Additional Tips:

- **VMware Tools Installation (Optional):**
  - Install VMware Tools for enhanced virtual machine performance.

- **Backup Virtual Machine:**
  - Periodically back up your virtual machine to avoid data loss.

- **Explore Ubuntu Documentation:**
  - Familiarize yourself with Ubuntu documentation for troubleshooting and best practices.





## Installation of C++ Compiler

## Step 1: Update Package Lists

1. **Open Terminal:**
   - Open a terminal on your Ubuntu system.

2. **Update Package Lists:**
   - Run the following commands to ensure your system has the latest package information:
     ```bash
     sudo apt update
     sudo apt upgrade
     ```



![image-20240201225244793](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20240201225244793.png)

## Step 2: Install GCC (GNU Compiler Collection)

1. **Install GCC:**

   - Run the following command to install the GNU Compiler Collection:
     ```bash
     sudo apt install build-essential
     ```

   ![image-20240201225517413](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20240201225517413.png)

1. **Verify Installation:**

   - Check the installed GCC version:
     ```bash
     g++ --version
     ```

## Step 3: Write and Compile a Simple Program

1. **Open Text Editor:**
   - Use your preferred text editor or an integrated development environment (IDE) to write a simple C++ program.

2. **Write C++ Code:**
   - Write a simple C++ program, for example, using `nano`:
     ```bash
     nano hello.cpp
     ```
     ```cpp
     #include <iostream>
     int main() {
         std::cout << "Hello, World!\n";
         return 0;
     }
     ```

3. **Save and Exit:**
   - Save the file and exit (`Ctrl + X`, press `Y`, and then press `Enter`).

4. **Compile and Execute:**
   - Compile the program using g++:
     ```bash
     g++ hello.cpp -o hello
     ```
   - Run the compiled executable:
     ```bash
     ./hello
     ```

## Additional Tips:

- **Integrated Development Environments (IDEs):**
  - Explore IDEs like Visual Studio Code, Code::Blocks, or CLion for a more feature-rich development environment.

- **C++ Build Systems:**
  - Learn about CMake or other build systems for managing complex C++ projects.

- **Additional Libraries:**
  - Install additional libraries if your projects require specific dependencies.

- **Online Compilers:**
  - Optionally, you can use online compilers for quick testing without installing on your local machine.







# Task2: Examples

## Example 1

In First Example we had to show the elements(Folders or Files) with their permissions.





![WhatsApp Image 2024-02-01 at 22.42.07_038ff237](C:\Users\HP\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\B7EE6F5F9AA5CD17CA1AEA43CE848496\WhatsApp Image 2024-02-01 at 22.42.07_038ff237.jpg)





## Example 2

In this Example we had to change the permissions of a file and show it.

![WhatsApp Image 2024-02-01 at 22.42.05_9a4f1e37](C:\Users\HP\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\4EA06FBC83CDD0A06020C35D50E1E89A\WhatsApp Image 2024-02-01 at 22.42.05_9a4f1e37.jpg)



