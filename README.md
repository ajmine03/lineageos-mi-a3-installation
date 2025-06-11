
# 📱 Successfully Installed LineageOS on Mi A3 (`laurel_sprout`)

I successfully installed a custom ROM (LineageOS) on my **Xiaomi Mi A3**. This repository documents my steps, resources, and troubleshooting tips. Hope this helps others flashing LineageOS or any other custom ROM on the Mi A3!

---

## 🔧 Device Info

- **Device Name**: Xiaomi Mi A3  
- **Codename**: `laurel_sprout`  
- **Bootloader**: Unlocked  
- **ROM**: LineageOS  
- **GApps**: [Yes/No] *(replace accordingly)*  
- **Rooted**: [Yes/No] *(replace accordingly)*

---

## 📚 Guide I Followed

- ✅ Official LineageOS Installation Guide for Mi A3:  
  👉 [https://wiki.lineageos.org/devices/laurel_sprout/install/](https://wiki.lineageos.org/devices/laurel_sprout/install/)

---

## 🛠️ Tools Used

| Tool | Description | Link |
|------|-------------|------|
| Platform Tools | ADB & Fastboot | [Download](https://developer.android.com/tools/releases/platform-tools) |
| LineageOS ROM | Official ROM Zip | [LineageOS Downloads](https://download.lineageos.org/) |
| Recovery Image | TWRP or Lineage Recovery | [Lineage Wiki](https://wiki.lineageos.org/devices/laurel_sprout/install/#installing-a-custom-recovery-using-fastboot) |
| GApps (Optional) | Google Apps | [OpenGApps](https://opengapps.org/) |
| Magisk (Optional) | Root Access | [Magisk GitHub](https://github.com/topjohnwu/Magisk) |

---

## 📝 Installation Steps (Simplified)

> ⚠️ **Backup everything** — your data will be wiped.

1. **Unlock Bootloader**
   ```bash
   fastboot oem unlock


2. **Flash Recovery**

   ```bash
   fastboot flash boot recovery.img
   

3. **Boot into Recovery**

4. **Wipe partitions**: `data`, `system`, `cache`

5. **Sideload LineageOS**

   ```bash
   adb sideload lineageos.zip
   ```

6. *(Optional)* Sideload **GApps** and/or **Magisk**

   ```bash
   adb sideload gapps.zip
   adb sideload magisk.zip
   ```

7. **Reboot & Setup**
   Your device should now boot into LineageOS!

---

## 🐞 Issues I Faced & Fixes

* **Bootloop after flashing**

  * *Fix*: Make sure to wipe `data`, `cache`, and `system` before flashing.
* **No Mobile Data**

  * *Fix*: Manually add APNs in Settings → Network → Mobile Network → Access Point Names

---

## 🔗 Helpful Links

* [LineageOS Official Site](https://lineageos.org/)
* [LineageOS Downloads](https://download.lineageos.org/)
* [OpenGApps](https://opengapps.org/)
* [Magisk GitHub](https://github.com/topjohnwu/Magisk)
* [XDA Mi A3 Forum](https://forum.xda-developers.com/f/xiaomi-mi-a3.9335/)

---

## 🤝 Credits

* ❤️ LineageOS Team
* 🙌 XDA Developers
* 🎥 YouTube tutorials
* 💬 Helpful forums & users

---

## ✍️ Author

**MD_AJMINE** 
Feel free to fork, star, or open issues if you need help!


