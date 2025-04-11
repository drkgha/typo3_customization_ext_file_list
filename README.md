This repository contains layout and template customizations for the TYPO3 extension [File List](https://github.com/xperseguers/t3ext-file_list/) by [Xavier Perseguers](https://github.com/xperseguers).

# 📸 Screenshot
![Image](https://github.com/user-attachments/assets/7a5f2ae1-444c-4caa-90fc-78e09e55dbac)

# 🔧 Requirements
* Typo3 *(Tested with TYPO3 v12.4)*
* Installed and configured File List extension by Xavier Perseguers *(Tested with File List v3.2.0)*
  
# 📦 Installation
1. Clone or download this repository into your TYPO3 project, for example into fileadmin/ or a suitable custom extension.

2. Add the following TypoScript configuration under Site Management > TypoScript > config (make sure to adjust the paths accordingly):
```
plugin.tx_filelist {
  view {
    templateRootPaths {
      10 = /webroot/customization/file_list/Templates/
    }
    partialRootPaths {
      10 = /webroot/customization/file_list/Partials/
    }
    layoutRootPaths {
      10 = /webroot/customization/file_list/Layouts/
    }
  }
}
```

3. Save the configuration and clear the caches.

# ⚠️ Notes
* Customizations are included for the **Simple Listing** layout only.
