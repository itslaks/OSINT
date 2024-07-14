

# OSINT



## Overview

OSINT (Open Source Intelligence) is a powerful tool designed to help you find social media usernames across multiple platforms based on user input. Leveraging the capabilities of the Sherlock Linux tool, OSINT automates the process of username discovery, making it easier to gather information for research, security analysis, and investigative purposes.

## Features

- **Username Search:** Find usernames on a wide range of social media platforms.
- **Batch Processing:** Input multiple usernames for bulk searches.
- **Customizable Searches:** Specify which platforms to include or exclude in the search.
- **Detailed Reports:** Generate comprehensive reports of findings.
- **Cross-Platform Support:** Compatible with Linux, macOS, and Windows.
- **Easy Integration:** Simple CLI interface for seamless integration into workflows.

## Table of Contents

1. [Getting Started](#getting-started)
2. [Installation](#installation)
3. [Usage](#usage)
   - [Basic Search](#basic-search)
   - [Advanced Search](#advanced-search)
   - [Batch Processing](#batch-processing)
4. [Configuration](#configuration)
5. [Examples](#examples)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)

## Getting Started

Follow these instructions to set up OSINT on your local machine and start finding social media usernames.

### Prerequisites

- Python 3.8 or higher
- Git

### Installation

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/itslaks/OSINT.git
    cd OSINT
    ```

2. **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Basic Search

Perform a basic search for a single username across multiple platforms:

```bash
python osint.py --username john_doe
```

### Advanced Search

Specify platforms for a more targeted search:

```bash
python osint.py --username john_doe --platforms twitter facebook instagram
```

### Batch Processing

Search for multiple usernames in one go by providing a file with usernames:

```bash
python osint.py --file usernames.txt
```

## Configuration

Customize the search behavior by editing the `config.json` file:

- **Timeouts:** Set the timeout duration for each request.
- **User-Agent:** Customize the User-Agent header for requests.
- **Platforms:** Add or remove platforms to search.

Example `config.json`:

```json
{
    "timeout": 10,
    "user_agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3",
    "platforms": ["twitter", "facebook", "instagram", "linkedin"]
}
```

## Examples

### Basic Example

Search for a username on all default platforms:

```bash
python osint.py --username jane_doe
```

### Specified Platforms

Search for a username only on Twitter and Instagram:

```bash
python osint.py --username jane_doe --platforms twitter instagram
```

### Batch Search

Search for usernames listed in `usernames.txt`:

```bash
python osint.py --file usernames.txt
```

## Contributing

We welcome contributions to OSINT! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch`
3. Make your changes.
4. Commit your changes: `git commit -m 'Add new feature'`
5. Push to the branch: `git push origin feature-branch`
6. Submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For questions, feedback, or collaboration opportunities, please reach out to us at:
- **Email:** contact@osinttool.com
- **GitHub Issues:** [Submit an issue](https://github.com/yourusername/OSINT/issues)

---

**OSINT** - Uncovering the digital footprint with ease





---

Discover the hidden social media presence with OSINT, and enhance your research and investigation capabilities. Join our community, contribute to our growth, and let's innovate together!
