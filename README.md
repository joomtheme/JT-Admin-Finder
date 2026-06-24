# JT Admin Finder

**JT Admin Finder** is a Joomla Administrator command palette extension built for **Joomla 6.1+** and the **Atum administrator template**.

It adds a fast `CTRL + K` shortcut inside Joomla Administrator, allowing administrators to quickly find and open common backend areas without navigating through menus.

---

## Features

* `CTRL + K` command palette for Joomla Administrator
* Joomla 6.1+ focused package
* Built for PHP 8.3+
* Designed for the default Atum administrator template
* Joomla MVC based administrator component
* System plugin integration
* Web Asset Manager based CSS and JavaScript loading
* ACL-aware Joomla core administrator links
* Keyboard-friendly modal interaction
* Improved URL validation for safer navigation
* GPL licensed package
* Joomla update server support
* Changelog metadata support
* SHA-256 checksum support for update packages

---

## Requirements

| Requirement            | Version      |
| ---------------------- | ------------ |
| Joomla                 | 6.1 or newer |
| PHP                    | 8.3 or newer |
| Administrator Template | Atum         |

---

## Installation

Download the latest package ZIP from the GitHub Releases page:

```text
pkg_jtadminfinder_v0.1.17.zip
```

Then install it from Joomla Administrator:

```text
System → Install → Extensions → Upload Package File
```

After installation, the system plugin is enabled automatically on first install.

---

## Usage

Open Joomla Administrator and press:

```text
CTRL + K
```

The JT Admin Finder command palette will appear.

Start typing to search for Joomla Administrator areas, then select an item to open it.

---

## Package Structure

JT Admin Finder is distributed as a Joomla package extension.

The package includes:

```text
pkg_jtadminfinder
├── com_jtadminfinder
└── plg_system_jtadminfinder
```

### Component

The administrator component provides the backend configuration and package integration.

```text
administrator/components/com_jtadminfinder
```

### Plugin

The system plugin loads the command palette inside Joomla Administrator.

```text
plugins/system/jtadminfinder
```

---

## Update Server

JT Admin Finder supports Joomla Extension Update.

The update server XML is located at:

```text
https://raw.githubusercontent.com/joomtheme/JT-Admin-Finder/main/updates/jtadminfinder.xml
```

The changelog XML is located at:

```text
https://raw.githubusercontent.com/joomtheme/JT-Admin-Finder/main/updates/changelog.xml
```

Although the extension works inside Joomla Administrator, the package extension record is matched by Joomla using the package entry in the extensions table.

---

## Current Release

### v0.1.17

This release focuses on Joomla 6.1+ update compatibility and package metadata cleanup.

Highlights:

* Joomla package update XML compatibility improved
* Clean package ZIP structure
* Fixed package metadata consistency

---

## Security

JT Admin Finder validates command palette URLs before navigation.

The command palette blocks unsafe schemes such as:

```text
javascript:
data:
vbscript:
```

It also avoids navigating to external administrator URLs.

---

## JED Checker

The package has been prepared with Joomla Extension Directory submission requirements in mind and has passed JED Checker testing.

Please note that passing JED Checker does not guarantee final Joomla Extensions Directory approval.

---

## License

JT Admin Finder is licensed under the **GNU General Public License v2 or later**.

See the `LICENSE.txt` file for details.

---

## Author

**JoomTheme**

Website:
https://joomtheme.com

Repository:
https://github.com/joomtheme/JT-Admin-Finder
