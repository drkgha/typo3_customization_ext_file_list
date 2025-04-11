This repository contains layout and template customizations for the TYPO3 extension **File List** by Xavier Perseguers.

# Requirements
* Typo3 *(Tested with TYPO3 v12.4)*
* Installed and configured File List extension by Xavier Perseguers *(Tested with File List v3.2.0)*
# Installation
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

**Note: Customizations are included for the Simple Listing layout only.**
