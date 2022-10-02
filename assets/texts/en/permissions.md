# Requested permissions

For a general explanation of add-on permissions see [this support article](https://support.mozilla.org/kb/permission-request-messages-firefox-extensions).

## Installation permissions

Currently, no permission is requested at the installation or when updating.

## Feature-specific (optional) permissions

These permissions are requested when doing some specific actions, if they are needed for that.

| Internal Id | Permission                                                        | Requested at…              | Explanation                                                                                                                                                                                       |
|:------------|:------------------------------------------------------------------|:---------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `downloads` | Download files and read and modify the browser’s download history | Download of QR code as SVG | Needed for downloading (saving) the SVG and allowing the user to choose a file location. This add-on does not access your downloaded files, it just uses this permission to start the download. |

## Hidden permissions
Additionally, it requests these permissions, which are not requested in Firefox when the add-on is installed, as they are not major permissions.

| Internal Id    | Permission                   | Explanation                                                       |
|:---------------|:-----------------------------|:------------------------------------------------------------------|
| `activeTab`    | Access current tab website   | Needed for getting the URL of the current website for the QR code |
| `storage`      | Access local storage         | Needed for saving options                                         |
| `menus`        | Modify browser context menus | Needed for adding context menus "QR code from selection" (etc.)   |
| `clipboardRead`| Access clipboard content     | Needed for using clipboard content to create QR code              |
