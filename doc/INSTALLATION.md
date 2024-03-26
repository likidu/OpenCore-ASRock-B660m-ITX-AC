# Installation notes

## Sonoma 14.4.1

Encountered balck screen after OpenCore picker and first installation with verbose. What I did was:

- Use the bottom DP on RX6600
- Remove `RadeonSensor.kext` and `SMCRadeon.kext`
- Remove `boot-args` `keepsyms=1 debug=0x100`
- Plug USB stick in the back ports