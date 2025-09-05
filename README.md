# MPPHA dual MPPT for ESPHome

📡 ESPHome firmware for **Voltronic MPPHA dual MPPT** inverters, ready to integrate with Home Assistant.

To be used with MPPHA electronic module made esspecially for this purpose

<img width="1152" height="1373" alt="image" src="https://github.com/user-attachments/assets/c60abaf0-473b-4760-b51d-8d6e90fadb3a" />


## 🚀 Features
- Full integration via [ESPHome](https://esphome.io)
- Automatic detection and adoption through **ESPHome Dashboard**
- Easy Wi-Fi provisioning (Improv over BLE + captive portal)
- Local Web UI on port 80
- Exposes sensors and controls: voltages, currents, temperature, device mode, charging priorities, and more
- OTA firmware updates

## 🛠️ Installation
1. Open **ESPHome Dashboard** in Home Assistant.
2. Choose **+ New Device** → **Adopt** → Import firmware: github://mchiriciuc/mppha-dual-mppt/firmware.yaml
3. Follow the steps to improv BLE or use the Captive portal 
4. Connect the device to Wi-Fi.

## 📦 Releases
Latest stable release:  
[firmware.yaml v1.0.0](https://github.com/mchiriciuc/mppha-dual-mppt/releases/tag/v1.0.0)

## 🔧 Advanced Configuration
- Parameters can be adjusted via Home Assistant (`select` and `number` entities).
- Recommended OTA secured configuration:
```yaml
api:
 encryption:
   key: "GENERATED_KEY"
ota:
 password: "STRONG_PASSWORD"
