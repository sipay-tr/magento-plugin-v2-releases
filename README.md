# Sipay Magento 2 Plugin — Releases

This repository hosts the official downloadable releases of the **Sipay Magento 2 payment module** — download a ready-to-install `.zip` from the [Releases](https://github.com/sipay-tr/magento-plugin-v2-releases/releases/latest) page.

## Download the latest release

1. Open the [**Releases**](https://github.com/sipay-tr/magento-plugin-v2-releases/releases/latest) page.
2. Download the **`sipay-magento-2-plugin-<version>.zip`** file attached to the latest release.

## Installation

The download is a standard Magento 2 module that installs under `app/code/Sipay/SipayPos`.

1. Download `sipay-magento-2-plugin-<version>.zip` from the latest release.
2. Extract it into your Magento project's `app/code/` directory. The archive already nests the module under `Sipay/SipayPos/`, so the files land at `app/code/Sipay/SipayPos/`.
3. From your Magento root directory, run:

   ```bash
   bin/magento setup:upgrade
   bin/magento setup:di:compile
   bin/magento cache:flush
   ```

   If your store runs in production mode, also deploy static content:

   ```bash
   bin/magento setup:static-content:deploy
   ```
4. In the Magento Admin, go to **Stores → Configuration → Sales → Payment Methods**, enable **Sipay**, and enter your Sipay API credentials.

> **Updating:** replace the contents of `app/code/Sipay/SipayPos/` with the newest release and re-run the commands above.

## Requirements

- A running **Magento 2** store (Open Source or Adobe Commerce).
- **PHP** compatible with your Magento 2 version.
- Command-line access to run `bin/magento` commands.
- A valid **Sipay merchant account** and API credentials.

## Support

For questions and integration support, please contact Sipay.
