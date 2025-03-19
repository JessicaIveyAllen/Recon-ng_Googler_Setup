# Recon-ng_Googler_Setup
This repository provides installation, configuration, and usage instructions for Recon-ng and Googler on Ubuntu for reconnaissance and OSINT (Open Source Intelligence) gathering.
# Recon-ng & Googler Setup on Ubuntu

## Overview
This repository provides installation, configuration, and usage instructions for **Recon-ng** and **Googler** on Ubuntu for reconnaissance and OSINT (Open Source Intelligence) gathering.

## Prerequisites
Ensure you have the following installed on your Ubuntu system:
- **Python 3**  
```bash
python3 --version
```
- **Git**  
```bash
sudo apt install git -y
```
- **Pip**  
```bash
sudo apt install python3-pip -y
```

## Installation

### Installing Recon-ng
1. Clone the **Recon-ng** repository:  
```bash
cd ~
rm -rf recon-ng
git clone https://github.com/lanmaster53/recon-ng.git
cd recon-ng
```
2. Create a Python virtual environment and install dependencies:  
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```
3. Run **Recon-ng**:  
```bash
./recon-ng
```

### Installing Googler
1. Update package lists:  
```bash
sudo apt update
```
2. Install **Googler**:  
```bash
sudo apt install googler -y
```
3. Verify installation:  
```bash
googler --version
```

## Usage

### Using Recon-ng
1. Start Recon-ng:  
```bash
./recon-ng
```
2. Show available modules:  
```bash
modules search
```
3. Load a module:  
```bash
modules load [module_name]
```
4. Set options and execute commands within Recon-ng.

### Using Googler for Google Dorking
1. Perform a site-specific search:  
```bash
googler site:example.com
```
2. Use a time delay to avoid rate limiting:  
```bash
googler --time=1 site:example.com
```
3. Test Googler configuration:  
```bash
googler ubuntu
```

### Exiting Googler
To exit **Googler**, press:  
```bash
Ctrl + C
```
## Credits
- [Recon-ng GitHub](https://github.com/lanmaster53/recon-ng)  
- [Googler GitHub](https://github.com/jarun/googler)

