# 4x4 Tenkey - Raspberry Pi Pico (RP2040)

Based on tenkey.kicad_pcb: rows GP1, GP2, GP4, GP5; columns GP6, GP7, GP9, GP10; diode direction COL2ROW.

## Build
1. Set up QMK environment: https://docs.qmk.fm/newbs_getting_started
2. Copy `keyboards/otto_tenkey` into `qmk_firmware/keyboards/`.
3. Run: `qmk compile -kb otto_tenkey -km default`
4. Find the generated `.uf2` in `qmk_firmware/`.
5. Hold BOOTSEL while connecting Pico over USB. Release BOOTSEL, then copy `.uf2` into RPI-RP2 drive.

These are source files, NOT a precompiled firmware UF2. Verify solder joints and absence of supply shorts before attaching USB.

Note: The VID/PID are placeholders for personal development; replace them with appropriate assigned identifiers before distribution.
