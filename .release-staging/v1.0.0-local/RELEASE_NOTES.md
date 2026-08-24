Preview release for supervised Geely EX2 testing.

Includes:

- Flyme Auto head-unit agent (minSdk 28)
- Android phone controller (minSdk 26)
- SHA-256 checksums

Changes in this updated preview:

- Rejects stale Flyme current and charge-state telemetry, preventing cached 4.7 A readings from falsely reporting AC charging.
- Keeps Start AC available for connected, stopped AC sessions after refresh when Flyme reports the stopped connector mode as unknown.
- Enables Start AC only while connected and stopped; enables Stop AC only while connected and charging.
- Hides untested manual DC Start/Stop controls.
- Disables Apply AC current until the selected current differs from the configured value.
- Disables the maximum-SOC percentage slider while the maximum-SOC rule is switched off.
- Retains local pairing, AC-current control, persistent maximum-SOC stopping, refresh controls, and controller activity history.

Install in update mode to preserve pairing and commissioning data.

Current artifact hashes:

- Agent: `4c80bb03f0a87a0a94d40bb2afcb83d4a30046f9883f648b8aa781b1fa72c09a`
- Controller: `39d2d09cf5212558fe6ec5b43af1232e9d61b9b776fa615598aec9b07b018601`

Unofficial, debug-signed preview software. Test while parked and supervised. Not affiliated with Geely, Flyme, Meizu, or ECARX. Application source code is not included in this repository.
