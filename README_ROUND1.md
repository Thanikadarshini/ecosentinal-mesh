# UrbanPulseX - EcoSentinel Mesh | Round 1

## Run the dashboard
1. Open this folder in VS Code.
2. Open PowerShell in the folder containing `package.json`.
3. Run `npm install`.
4. Run `npm run dev`.
5. Open the localhost URL shown by Vite.

## PDF report
Use **DOWNLOAD REPORT** at the top-right or **Download PDF Report** in Analytics. The PDF contains current sensor telemetry, risk scores, connectivity/resilience status, recent telemetry packets, response shelters, and system flow.

The report is generated in the browser and downloads directly as a `.pdf`; no Excel/CSV export is used for the report feature.

## ESP32
Firmware is in `esp32_ecosentinel_mesh/EcoSentinel_Mesh.ino`.
Serial: 115200 baud. The dashboard expects one JSON telemetry packet per line with `type: telemetry`.

## Prototype note
The MQ-2 is used as an air-quality/smoke proxy for this prototype. It is not a calibrated AQI instrument.
