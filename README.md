# Recon-ng Googler Setup

## Overview

The **Recon-ng Googler Setup** repository is designed to streamline and automate the process of conducting Google Dorking using the powerful Recon-ng framework. This setup leverages Recon-ng's modular design to efficiently gather open-source intelligence (OSINT) data for cybersecurity research and penetration testing.

## Features

- 🛠️ Automated Google Dorking with tailored search queries
- ⚙️ Easy-to-use modules for various OSINT data points
- 🔍 Flexible keyword and URL customization for precision targeting
- 📋 Integrated reporting for organized data collection

## Prerequisites

Before you begin, ensure you have the following:

- 🐍 **Python 3.8+**
- 🧰 **Recon-ng** installed (`pip install recon-ng`)
- 📄 **Google Dorks Query List** (included in the repository)
- 💻 Access to a terminal or command-line interface

## Installation

1. 📥 Clone this repository:
   ```bash
   git clone https://github.com/JessicaIveyAllen/Recon-ng_Googler_Setup.git
   cd Recon-ng_Googler_Setup
   ```
2. 📦 Install Recon-ng dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. 🚀 Launch Recon-ng:
   ```bash
   recon-ng
   ```

## Usage

1. 🔌 Load the **google_dorker** module:
   ```bash
   modules load recon/domains-contacts/google_dorker
   ```
2. ⚙️ Set the required options:
   ```bash
   options set SOURCE yourtarget.com
   options set QUERY_LIST ./dorks.txt
   ```
3. ▶️ Run the module:
   ```bash
   run
   ```

## Google Dorks Query List

The `dorks.txt` file includes essential queries like:

- 🛡️ **`site:target.com inurl:admin`** - Identify admin portals
- 📂 **`site:target.com filetype:pdf`** - Locate public-facing PDFs
- 📁 **`intitle:index.of`** - Expose directory listings

## Reporting

- 📋 Results are automatically saved in `/results/`.
- 📊 Output formats include `.csv` and `.json` for flexibility in analysis and presentation.

## Best Practices

- ⚠️ Respect legal boundaries when using Google Dorking for reconnaissance.
- 🧑‍💻 Prioritize ethical hacking principles and obtain authorization before targeting any domain.

## Contributing

🖋️ Contributions are welcome! Feel free to submit pull requests with new dork queries, module improvements, or bug fixes.

## License

📜 This project is licensed under the **MIT License**.

## Contact

📫 For questions, suggestions, or issues, please reach out via [GitHub](https://github.com/JessicaIveyAllen).

## Installing Recon-ng

1. 📥 Clone the Recon-ng repository:
   ```bash
   cd ~
   rm -rf recon-ng
   git clone https://github.com/lanmaster53/recon-ng.git
   cd recon-ng
   ```
2. 🐍 Create a Python virtual environment and install dependencies:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```
3. 🚀 Run Recon-ng:
   ```bash
   ./recon-ng
   ```

## Installing Googler

1. 🔄 Update package lists:
   ```bash
   sudo apt update
   ```
2. 📦 Install Googler:
   ```bash
   sudo apt install googler -y
   ```
3. ✔️ Verify installation:
   ```bash
   googler --version
   ```

## Usage

### Using Recon-ng

1. 🚀 Start Recon-ng:
   ```bash
   ./recon-ng
   ```
2. 🔍 Show available modules:
   ```bash
   modules search
   ```
3. 🔌 Load a module:
   ```bash
   modules load [module_name]
   ```
4. ⚙️ Set options and execute commands within Recon-ng.

### Using Googler for Google Dorking

1. 🌐 Perform a site-specific search:
   ```bash
   googler site:example.com
   ```
2. ⏲️ Use a time delay to avoid rate limiting:
   ```bash
   googler --time=1 site:example.com
   ```
3. 🧪 Test Googler configuration:
   ```bash
   googler ubuntu
   ```

### Exiting Googler

To exit Googler, press:

🛑 **Ctrl + C**

