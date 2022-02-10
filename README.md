# PSoC 6 MCU: 

CY8C6245

## CUSTOM BSP SETUP (device Selection)

- [Creating Custom BSP](https://community.infineon.com/t5/Knowledge-Base-Articles/Creating-Custom-BSPs-in-ModusToolbox-KBA230822/ta-p/251741) v2.2

on modus-shell open project directory (same folder as make file) or terminal inside modustoolbox run:

```
make bsp TARGET_GEN=PSOC6245 DEVICE_GEN=CY8C6245FNI-S3D41
```
right click project
select Build targets -> Create

type into Target Name
```
bsp TARGET_GEN=PSOC6245 DEVICE_GEN=CY8C6245FNI-S3D41
```

modify the make file replace PSOC6-GENERIC with the TARGET_GEN above

```
TARGET=PSOC6-GENERIC
```

```
TARGET=PSOC6245
```

run build to verify