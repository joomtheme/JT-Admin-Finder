# JT Admin Finder

**JT Admin Finder** is a Joomla Administrator command palette extension built for **Joomla 6.1+**, **PHP 8.3+**, and the **Atum administrator template**.

It adds a fast keyboard-driven command palette inside Joomla Administrator, allowing administrators to quickly find and open common backend areas without navigating through menus.

Use **Ctrl + K** on Windows/Linux or **Cmd + K** on macOS to open the command palette.

---

## Features

* Command palette for Joomla Administrator
* `Ctrl + K` shortcut for Windows/Linux
* `Cmd + K` shortcut for macOS
* Joomla native keyboard shortcut support with `J` then `K`
* Joomla 6.1+ focused package
* PHP 8.3+ requirement
* Designed for the default Atum administrator template
* Joomla MVC based administrator component
* System plugin integration
* Web Asset Manager based CSS and JavaScript loading
* ACL-aware Joomla core administrator links
* Keyboard-friendly modal interaction
* Improved accessibility and focus handling
* Improved URL validation for safer navigation
* GPL licensed package
* Joomla update server support
* Changelog metadata support
* SHA-256 checksum support for update packages
* System plugin auto-enabled only on first install

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

During updates, JT Admin Finder does not force-enable the plugin again, so existing administrator preferences are respected.

---

## Usage

Open Joomla Administrator and press:

```text
Ctrl + K
```

on Windows/Linux, or:

```text
Cmd + K
```

on macOS.

The JT Admin Finder command palette will appear.

You can also use Joomla’s native keyboard shortcut system:

```text
J then K
```

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

The administrator component provides the backend dashboard and package integration.

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

JT Admin Finder supports Joomla Extension Update through the package manifest.

The update server XML is located at:

```text
https://raw.githubusercontent.com/joomtheme/JT-Admin-Finder/main/updates/jtadminfinder.xml
```

The changelog XML is located at:

```text
https://raw.githubusercontent.com/joomtheme/JT-Admin-Finder/main/updates/changelog.xml
```

Package updates are managed through the package extension record.

---

## Current Release

### v0.1.17

This release focuses on Joomla 6.1+ compatibility, package metadata cleanup, update server handling, and JED submission preparation.

Highlights:

* Joomla 6.1+ and PHP 8.3+ focused release
* Package, component, plugin, asset, update, and changelog metadata updated to v0.1.17
* Full GPL license file included
* Web Asset Manager asset versions aligned with the release version
* Package update server metadata added
* SHA-256 checksum metadata added for package update verification
* Changelog metadata support added
* Update handling cleaned so updates are managed through the package manifest
* System plugin auto-enabled only on first install
* Plugin state is not forced again during updates
* ACL filtering improved for Joomla core administrator links
* URL validation hardened for command palette navigation
* Modal accessibility, keyboard behaviour, and focus handling improved

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
