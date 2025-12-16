# WHMCS Twenty-One Theme - Dark Mode (Custom CSS)

This is a customized CSS file that transforms the default WHMCS **Twenty-One** theme into a full Dark Mode.

This solution overrides the default theme colors using the `custom.css` file, meaning it does not require modifying core template files and is persistent through WHMCS updates (as long as the `custom.css` file is preserved).

## Features

This stylesheet corrects and darkens the following areas that often remain white by default:

* **General Look:** Dark background (#121212) and light text.
* **Navigation:** Top Bar, Main Navbar, and Footer.
* **Dashboard:** Homepage tiles (Services, Domains, Tickets), "Active Products" cards, and sidebars.
* **Tables:** Dark backgrounds for tables, corrected header rows, and text colors.
* **Pagination:** Fixed "Previous" and "Next" buttons (no longer white blocks).
* **Forms:** Input fields, dropdowns, and search bars.
* **Specific Fixes:**
    * Removes white backgrounds from "Why Choose Us" marketing blocks.
    * Fixes the Domain Search background area on the homepage.
    * Darkens the "Breadcrumb" bar (Secondary Header).

## Installation

1.  Download the `custom.css` file from this repository.
2.  Log in to your server (via FTP or File Manager).
3.  Navigate to the directory:
    ```
    /path_to_whmcs/templates/twenty-one/css/
    ```
4.  Upload the `custom.css` file to this folder.
    * *Note:* If a `custom.css` file already exists, backup your current file and append the content of this file to the end, or replace it entirely if preferred.

## Usage (Important!)

For the changes to take effect, you **must** clear the WHMCS internal cache. Simply refreshing your browser is usually not enough.

1.  Log in to the WHMCS Admin Area.
2.  Go to **Utilities** > **System** > **System Cleanup**.
3.  Click **Go** next to **Empty Template Cache**.
4.  Clear your browser cache or open your Client Area in an Incognito/Private window to see the changes.

## Troubleshooting

**Problem:** Some boxes are still white.
**Solution:** Ensure you uploaded the file to the correct folder (`templates/twenty-one/css/`). If you are using a Child Theme, the path might differ. Remember to empty the *Template Cache* from the Admin Area.

**Problem:** The logo is not visible on the dark background.
**Solution:** The CSS file includes a small fix (`.navbar-brand img`) that adds a small white background/border to the logo. For the best result, we recommend using a light version of your logo (.png or .svg) with a transparent background.

## License

This project is licensed under the **GNU General Public License v3.0 (GPLv3)**.
See the [LICENSE](LICENSE) file for details.
