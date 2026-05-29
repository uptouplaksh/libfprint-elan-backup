# ELAN Fingerprint Sensor Working Configuration

Date: 2026-05-29

## Hardware
Sensor: ELAN Match-on-Chip 2
USB ID: 04f3:0c00

## Repository
Branch: elanmoc2-working
Commit: 3d489ebea22b2d6fb740cd9ee2decbacf1afe635

## Status
- Fingerprint enrollment working
- Fingerprint login working
- Passkeys working

## Recovery

git checkout 3d489ebea22b2d6fb740cd9ee2decbacf1afe635

Then rebuild:

meson setup builddir --prefix=/usr
cd builddir
meson compile
sudo meson install
sudo ldconfig

