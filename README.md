[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=social&logo=linkedin)](https://www.linkedin.com/in/mihail-ziablitsev-2109a42a0/)

# Developer Configuration in Production Mode

A custom Magento 2 module that restores **developer-oriented configuration settings** even when the store is running in **production mode**.  

Normally, Magento restricts certain developer features for performance and security reasons in production.  
This module allows developers to **temporarily re-enable specific settings** without switching the whole store to developer mode.  

---

## Features
- Restores **developer settings** in production environments.  
- Useful for debugging and testing on staging/live-like environments.  
- Avoids constant switching between developer and production modes.  
- Lightweight and safe — only targeted developer configurations are restored.  

### Restored Configuration (by default)
- **Template Hints** (`dev/debug/template_hints`)  
- **Template Hints in Admin** (`dev/debug/template_hints_admin`)  
- **Inline Translation** (`dev/translate_inline/active`)  
- **Static Asset Signing** (`dev/static/sign`)  
- **Developer Logging / Profiler options** (`dev/debug/debug_logging`, `dev/debug/profiler`)  

---

## Installation

1. Require the module via Composer:

```bash
composer require mizir/developer-configuration-in-production-mode
```

## Usage

Once installed, the module will restore developer-related configuration settings automatically in production mode.

You can check applied values in the admin panel under:
Stores → Configuration → Advanced → Developer
