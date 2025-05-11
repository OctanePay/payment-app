---
title: OctanePay Payment App
description: A payment application for Android-based EDC devices to accept cryptocurrency payments via NFC tap-to-pay from cold wallets.
---

import { CodeBlock } from '@theme/CodeBlock';

# OctanePay Payment App

**OctanePay** is a payment application designed for Android-based Electronic Data Capture (EDC) devices, enabling merchants to accept cryptocurrency payments using NFC tap-to-pay from customers' cold wallets. Merchants must configure a receiving address for payments, ensuring secure and seamless transactions. OctanePay bridges traditional point-of-sale (POS) systems with blockchain technology, empowering businesses to engage with the cryptocurrency economy.

## Features

- **NFC Tap-to-Pay**: Accept payments from cold wallets stored on NFC-enabled cards with a simple tap on the EDC device.
- **Merchant Address Configuration**: Merchants set a unique cryptocurrency receiving address before processing payments.
- **User-Friendly Interface**: Intuitive EDC interface for merchants to manage transactions with minimal training.
- **Receipt Generation**: Prints or emails transaction receipts with QR codes for blockchain verification.
- **Multi-Network Support**: Supports payments across multiple blockchain networks (e.g., Bitcoin, Ethereum, Solana).

## Supported Cryptocurrencies

- Bitcoin (BTC)
- Ethereum (ETH)
- Solana (SOL)

> **Note**: More tokens can be added via API updates. See [API Integration](#api-integration).

## Requirements

- **Hardware**: Android-based EDC device with NFC reader, touchscreen, and internet connectivity (Wi-Fi or mobile data).
- **Software**:
  - OctanePay Payment App APK (version 1.0.0 or later).
  - Android OS (version 7.0 or higher).
- **Customer Hardware**: NFC-enabled card with a cold wallet supporting tap-to-pay (e.g., compatible with Bitcoin or Ethereum protocols).

## Installation

1. **Download the APK**:
   - Obtain the OctanePay APK from the official [OctanePay website](https://octanepay.com/downloads) or your EDC provider’s portal.
   - Verify the APK’s digital signature to ensure authenticity.

2. **Enable Unknown Sources**:
   - On the EDC device, navigate to `Settings > Security`.
   - Enable `Install from Unknown Sources` to allow APK installation.

3. **Install the APK**:
   - Transfer the APK to the EDC device via USB, Bluetooth, or direct download.
   - Open the APK file and follow the on-screen prompts to install.

   <CodeBlock language="bash">
     # Example: Install via ADB (if connected to a computer)
     adb install octanepay_1.0.0.apk
   </CodeBlock>

4. **Verify Installation**:
   - Launch the OctanePay App from the EDC’s app drawer.
   - Ensure the app version matches the latest release (1.0.0 or higher).

## Setup

1. **Set Receiving Address**:
   - In the OctanePay App, navigate to `Settings > Payment Address`.
   - Enter or generate a cryptocurrency wallet address for each supported currency (e.g., BTC, ETH).
   - Verify the address to ensure it is correctly linked to the merchant’s wallet.

2. **Configure NFC**:
   - Ensure the EDC’s NFC reader is enabled (`Settings > NFC > On`).
   - Test NFC functionality by tapping a compatible card to confirm detection.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
