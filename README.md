# How-to-install-Gline-Jar-modules 📖

[![Free guide](https://img.shields.io/badge/Free_guide-brightgreen)](LICENSE)
[![Contact](https://img.shields.io/badge/Contact-WhatsApp-brightgreen)](https://wa.me/8613801909968)

> **Free guide: how to install and activate Gline JAR modules on your Niagara Station.**

---

## What You'll Need

- A Niagara 4.14+ station (JACE, Edge, or Supervisor)
- The `.jar` module file from any Gline repository
- The `gline.pem` certificate file

---

## Installation Steps

### Step 1: Install the Certificate

1. Copy `gline.pem` to your station's user trust store
2. In Workbench: **Tools → User Trust Store → Import**
3. Select `gline.pem` and confirm

### Step 2: Deploy the Module

1. Copy the `.jar` file to your Niagara `modules/` directory
   - Typical path: `C:\Niagara\Niagara-4.x.x\modules\`
   - JACE path: `/niagara/modules/`
2. Restart the station

### Step 3: Verify Installation

1. Open Workbench → **Palette**
2. Search for the module name (e.g., `glineFtpServer`, `bogSnap`)
3. If visible, the module is installed and signed correctly

> ⚠️ **Certificate issue?** If the module doesn't appear, the `gline.pem` certificate may not be properly installed. Contact us for assistance with custom certificate signing.

---

## Troubleshooting

| Symptom | Solution |
|---------|----------|
| Module not in Palette | Re-install gline.pem certificate |
| JAR not found in modules/ | Check the modules directory path |
| Permission error | Ensure station is restarted |
| Trial license expired | Email us for extension |

---

## Custom Certificate Signing

If your organization requires a certificate signed with your own key instead of gline.pem:

1. Provide us with your certificate file (`.pem`) and password
2. We recompile and re-sign the JAR with your certificate
3. Deploy the custom-signed JAR — no external certificate installation needed

---

## Support & Contact

- **Email**: [jason.zhang@gline-net.com](mailto:jason.zhang@gline-net.com)
- **WhatsApp**: [+86 138 0199 0968](https://wa.me/8613801909968)

**Shanghai Gline Net Co., Ltd.** — Your Partner in Smarter Automation

Step 1: install the gline.pem into workbench
Click Tools and select Certificate Management. Click the User Trust Store and import the gline certificate file.
<img width="2687" height="613" alt="image" src="https://github.com/user-attachments/assets/a7e22843-cc3b-4b93-8f41-d96aefe4503c" />

Step 2: install gline.pem into station platform
Even in the same PC where has installed gline.pem in workbench, this step is still mandatory.
Go to Platform and click the Certificate Management. Then click the User Trust Store. Import the gline certificate file again. 
<img width="1899" height="413" alt="image" src="https://github.com/user-attachments/assets/b9ca0742-f7ac-4cb1-aba5-7d5638f5e2fc" />

Step 3: close the workbench and add the gline modules into the workbench module folder. 

Step 4: install the platform daemon. This will adopt the new certificate to the workbench. 

Step 5: install the gline module into the Niagara station module. This is similar to other 3rd jar module import porcess. Go the platform and software manager and import the module file. Then reboot the station. 
If the station is running as supervisor at the same workbench, this step is not necessary. 

With above steps, you could then enjoy our modules. 

If you have any issue, feel free to contact with me jason.zhang@gline-net.com


