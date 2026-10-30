
# Lab 01 - Ubuntu Server Virtualization

## Objective
Deploy Ubuntu Server using Oracle VirtualBox
to practice Linux system administration,
networking, and MySQL.

## Hardware Configuration

| Component | Configuration |
|---|---|
| Host OS | Windows 11 |
| Hypervisor | Oracle VirtualBox |
| VM Name | Ubuntu-Server-Lab |
| Guest OS | Ubuntu Server 26.04.1 LTS |
| RAM | 4096 MB |
| vCPUs | 2 |
| Virtual Disk | 40 GB |
| Firmware | UEFI |
| Installation | Manual |

## Progress

- [x] Downloaded Ubuntu Server ISO
- [x] Selected the ISO in VirtualBox
- [ ] Confirm hardware configuration
- [ ] Install Ubuntu Server
- [ ] Verify system installation
- [ ] Configure networking
- [ ] Install MySQL


## Troubleshooting

### Multipath warning during boot

During the initial Ubuntu Server boot,
the following error was observed:

ERROR: bad settings in read-only bindings file
/etc/multipath/bindings

The error appears to affect the multipath
storage component during early boot.

Status: Under investigation.

Next step: Verify whether the Ubuntu Server
installer starts successfully.


## Troubleshooting

### Issue 01 - Ubuntu Server boot freeze

**Environment:** Ubuntu Server 26.04.1 LTS
running in Oracle VirtualBox.

**Observed behavior:**
The installation process stopped at:

`Begin: Loading essential drivers ...`

A multipath configuration error was also
displayed during startup.

**Investigation:**
Similar boot freezes have been reported
with VirtualBox and Ubuntu.

**Test 01:**
Pause and resume the virtual machine.

**Result:** Pending verification.

**Status:** Under investigation.





### Test 01 - Pause and Resume Virtual Machine

**Action performed:**
Paused the Ubuntu Server virtual machine
using VirtualBox and then resumed execution.

**Result: SUCCESS**

The system continued its boot process and
successfully displayed the Ubuntu Server
language selection screen.

**Observation:**
The workaround restored progress during
installation, but the underlying cause of
the initial freeze has not been confirmed.

**Status:** Boot workaround successful.
Ubuntu Server installation in progress.
