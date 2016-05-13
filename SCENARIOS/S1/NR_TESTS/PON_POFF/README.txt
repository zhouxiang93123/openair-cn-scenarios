This scenario capture was realized in EURECOM with:

################################################################################
- a NEXUS 5 phone, 10 meters away from eNB antennas (see for frequencies, etc: enb.conf)
GSM 850/900/1800/1900 WCDMA 800/850/900/1700/1900/2100 LTE 800/850/900/1800/2100/2600
ANDROID version 6.01
Baseband version M8974A-2.0.50.2.28
################################################################################



################################################################################
- a eNB running on a brick (eurecom ref: abeille):
################################################################################
  OPENAIR CODE:
    repository: openairinterface5g
    commit 697c35dba37c89d632890014ff9e9dcd50cf4774
    Merge: 4af4848 92b07c8
    Author: Rohit Gupta <rohit.gupta@eurecom.fr>
    Date:   Wed Apr 6 12:05:10 2016 +0200

  LINUX:
    DISTRIB_ID=Ubuntu
    DISTRIB_RELEASE=14.04
    DISTRIB_CODENAME=trusty
    DISTRIB_DESCRIPTION="Ubuntu 14.04.2 LTS"

  KERNEL:     Linux ABEILLE 3.19.0-28-lowlatency #30~14.04.1-Ubuntu SMP PREEMPT Tue Sep 1 10:24:39 UTC 2015 x86_64 x86_64 x86_64 GNU/Linux

  RFCARD:     USRP B210
  CPU:        model name Intel(R) Core(TM) i7-4770R CPU @ 3.20GHz
  MEMORY:     16GB

  OTHER HARDWARE:
00:00.0 Host bridge: Intel Corporation Crystal Well DRAM Controller (rev 08)
	Subsystem: Gigabyte Technology Co., Ltd Device 5000
	Flags: bus master, fast devsel, latency 0
	Capabilities: <access denied>

00:02.0 VGA compatible controller: Intel Corporation Device 0d22 (rev 08) (prog-if 00 [VGA controller])
	Subsystem: Gigabyte Technology Co., Ltd Device d000
	Flags: bus master, fast devsel, latency 0, IRQ 33
	Memory at f7800000 (64-bit, non-prefetchable) [size=4M]
	Memory at e0000000 (64-bit, prefetchable) [size=256M]
	I/O ports at f000 [size=64]
	Expansion ROM at <unassigned> [disabled]
	Capabilities: <access denied>
	Kernel driver in use: i915

00:03.0 Audio device: Intel Corporation Crystal Well HD Audio Controller (rev 08)
	Subsystem: Gigabyte Technology Co., Ltd Device 5000
	Flags: bus master, fast devsel, latency 0, IRQ 35
	Memory at f7e14000 (64-bit, non-prefetchable) [size=16K]
	Capabilities: <access denied>
	Kernel driver in use: snd_hda_intel

00:14.0 USB controller: Intel Corporation 8 Series/C220 Series Chipset Family USB xHCI (rev 05) (prog-if 30 [XHCI])
	Subsystem: Gigabyte Technology Co., Ltd Device 5004
	Flags: bus master, medium devsel, latency 0, IRQ 29
	Memory at f7e00000 (64-bit, non-prefetchable) [size=64K]
	Capabilities: <access denied>
	Kernel driver in use: xhci_hcd

00:16.0 Communication controller: Intel Corporation 8 Series/C220 Series Chipset Family MEI Controller #1 (rev 04)
	Subsystem: Gigabyte Technology Co., Ltd Device 5001
	Flags: bus master, fast devsel, latency 0, IRQ 32
	Memory at f7e1e000 (64-bit, non-prefetchable) [size=16]
	Capabilities: <access denied>
	Kernel driver in use: mei_me

00:1a.0 USB controller: Intel Corporation 8 Series/C220 Series Chipset Family USB EHCI #2 (rev 05) (prog-if 20 [EHCI])
	Subsystem: Gigabyte Technology Co., Ltd Device 5004
	Flags: bus master, medium devsel, latency 0, IRQ 16
	Memory at f7e1c000 (32-bit, non-prefetchable) [size=1K]
	Capabilities: <access denied>
	Kernel driver in use: ehci-pci

00:1b.0 Audio device: Intel Corporation 8 Series/C220 Series Chipset High Definition Audio Controller (rev 05)
	Subsystem: Gigabyte Technology Co., Ltd Device fa50
	Flags: bus master, fast devsel, latency 0, IRQ 34
	Memory at f7e10000 (64-bit, non-prefetchable) [size=16K]
	Capabilities: <access denied>
	Kernel driver in use: snd_hda_intel

00:1c.0 PCI bridge: Intel Corporation 8 Series/C220 Series Chipset Family PCI Express Root Port #1 (rev d5) (prog-if 00 [Normal decode])
	Flags: bus master, fast devsel, latency 0
	Bus: primary=00, secondary=01, subordinate=01, sec-latency=0
	I/O behind bridge: 00002000-00002fff
	Memory behind bridge: df200000-df3fffff
	Prefetchable memory behind bridge: 00000000df400000-00000000df5fffff
	Capabilities: <access denied>
	Kernel driver in use: pcieport

00:1c.2 PCI bridge: Intel Corporation 8 Series/C220 Series Chipset Family PCI Express Root Port #3 (rev d5) (prog-if 00 [Normal decode])
	Flags: bus master, fast devsel, latency 0
	Bus: primary=00, secondary=02, subordinate=02, sec-latency=0
	I/O behind bridge: 0000e000-0000efff
	Memory behind bridge: f7d00000-f7dfffff
	Capabilities: <access denied>
	Kernel driver in use: pcieport

00:1c.3 PCI bridge: Intel Corporation 8 Series/C220 Series Chipset Family PCI Express Root Port #4 (rev d5) (prog-if 00 [Normal decode])
	Flags: bus master, fast devsel, latency 0
	Bus: primary=00, secondary=03, subordinate=03, sec-latency=0
	I/O behind bridge: 0000d000-0000dfff
	Memory behind bridge: f7c00000-f7cfffff
	Prefetchable memory behind bridge: 00000000f0000000-00000000f00fffff
	Capabilities: <access denied>
	Kernel driver in use: pcieport

00:1d.0 USB controller: Intel Corporation 8 Series/C220 Series Chipset Family USB EHCI #1 (rev 05) (prog-if 20 [EHCI])
	Subsystem: Gigabyte Technology Co., Ltd Device 5004
	Flags: bus master, medium devsel, latency 0, IRQ 23
	Memory at f7e1b000 (32-bit, non-prefetchable) [size=1K]
	Capabilities: <access denied>
	Kernel driver in use: ehci-pci

00:1f.0 ISA bridge: Intel Corporation HM87 Express LPC Controller (rev 05)
	Subsystem: Gigabyte Technology Co., Ltd Device 5001
	Flags: bus master, medium devsel, latency 0
	Capabilities: <access denied>
	Kernel driver in use: lpc_ich

00:1f.2 SATA controller: Intel Corporation 8 Series/C220 Series Chipset Family 6-port SATA Controller 1 [AHCI mode] (rev 05) (prog-if 01 [AHCI 1.0])
	Subsystem: Gigabyte Technology Co., Ltd Device b002
	Flags: bus master, 66MHz, medium devsel, latency 0, IRQ 30
	I/O ports at f0b0 [size=8]
	I/O ports at f0a0 [size=4]
	I/O ports at f090 [size=8]
	I/O ports at f080 [size=4]
	I/O ports at f060 [size=32]
	Memory at f7e1a000 (32-bit, non-prefetchable) [size=2K]
	Capabilities: <access denied>
	Kernel driver in use: ahci

00:1f.3 SMBus: Intel Corporation 8 Series/C220 Series Chipset Family SMBus Controller (rev 05)
	Subsystem: Gigabyte Technology Co., Ltd Device 5001
	Flags: medium devsel, IRQ 3
	Memory at f7e19000 (64-bit, non-prefetchable) [size=256]
	I/O ports at f040 [size=32]

02:00.0 Network controller: Realtek Semiconductor Co., Ltd. RTL8821AE 802.11ac PCIe Wireless Network Adapter
	Subsystem: AzureWave Device 2161
	Flags: bus master, fast devsel, latency 0, IRQ 3
	I/O ports at e000 [size=256]
	Memory at f7d00000 (64-bit, non-prefetchable) [size=16K]
	Capabilities: <access denied>

03:00.0 Ethernet controller: Realtek Semiconductor Co., Ltd. RTL8111/8168/8411 PCI Express Gigabit Ethernet Controller (rev 0c)
	Subsystem: Gigabyte Technology Co., Ltd Motherboard
	Flags: bus master, fast devsel, latency 0, IRQ 31
	I/O ports at d000 [size=256]
	Memory at f7c00000 (64-bit, non-prefetchable) [size=4K]
	Memory at f0000000 (64-bit, prefetchable) [size=16K]
	Capabilities: <access denied>
	Kernel driver in use: r8169

################################################################################
- EPC running on a desktop computer (eurecom ref: yang):
################################################################################
  OPENAIR CODE:
    repository openair-cn branch "unstable"
    commit 8a4917dbc2797feff64bcf012b708e814250f38a
    Author: gauthier <lionel.gauthier@eurecom.fr>
    Date:   Fri May 13 01:10:23 2016 +0200

  LINUX:
    DISTRIB_ID=Ubuntu
    DISTRIB_RELEASE=14.04
    DISTRIB_CODENAME=trusty
    DISTRIB_DESCRIPTION="Ubuntu 14.04.4 LTS"

  KERNEL:     Linux yang 3.19.0-28-generic #30~14.04.1-Ubuntu SMP Tue Sep 1 09:32:55 UTC 2015 x86_64 x86_64 x86_64 GNU/Linux

  RFCARD:     USRP B210
  CPU:        model name  : Intel(R) Core(TM) i7 CPU         950  @ 3.07GHz
  MEMORY:     4GB

  OTHER HARDWARE:
00:00.0 Host bridge: Intel Corporation 2nd Generation Core Processor Family DRAM Controller (rev 09)
    Subsystem: ASUSTeK Computer Inc. Device 105c
    Flags: bus master, fast devsel, latency 0
    Capabilities: <access denied>

00:01.0 PCI bridge: Intel Corporation Xeon E3-1200/2nd Generation Core Processor Family PCI Express Root Port (rev 09) (prog-if 00 [Normal decode])
    Flags: bus master, fast devsel, latency 0, IRQ 24
    Bus: primary=00, secondary=01, subordinate=01, sec-latency=0
    I/O behind bridge: 0000e000-0000efff
    Memory behind bridge: f6000000-f70fffff
    Prefetchable memory behind bridge: 00000000e0000000-00000000f1ffffff
    Capabilities: <access denied>
    Kernel driver in use: pcieport

00:02.0 VGA compatible controller: Intel Corporation 2nd Generation Core Processor Family Integrated Graphics Controller (rev 09) (prog-if 00 [VGA controller])
    DeviceName:  Onboard IGD
    Subsystem: ASUSTeK Computer Inc. Device 105c
    Flags: bus master, fast devsel, latency 0, IRQ 35
    Memory at f7400000 (64-bit, non-prefetchable) [size=4M]
    Memory at d0000000 (64-bit, prefetchable) [size=256M]
    I/O ports at f000 [size=64]
    Expansion ROM at <unassigned> [disabled]
    Capabilities: <access denied>
    Kernel driver in use: i915

00:16.0 Communication controller: Intel Corporation 6 Series/C200 Series Chipset Family MEI Controller #1 (rev 04)
    Subsystem: ASUSTeK Computer Inc. Device 105c
    Flags: bus master, fast devsel, latency 0, IRQ 37
    Memory at f7a0b000 (64-bit, non-prefetchable) [size=16]
    Capabilities: <access denied>
    Kernel driver in use: mei_me

00:1a.0 USB controller: Intel Corporation 6 Series/C200 Series Chipset Family USB Enhanced Host Controller #2 (rev 05) (prog-if 20 [EHCI])
    Subsystem: ASUSTeK Computer Inc. Device 105c
    Flags: bus master, medium devsel, latency 0, IRQ 16
    Memory at f7a08000 (32-bit, non-prefetchable) [size=1K]
    Capabilities: <access denied>
    Kernel driver in use: ehci-pci

00:1b.0 Audio device: Intel Corporation 6 Series/C200 Series Chipset Family High Definition Audio Controller (rev 05)
    Subsystem: ASUSTeK Computer Inc. Device 105c
    Flags: bus master, fast devsel, latency 0, IRQ 38
    Memory at f7a00000 (64-bit, non-prefetchable) [size=16K]
    Capabilities: <access denied>
    Kernel driver in use: snd_hda_intel

00:1c.0 PCI bridge: Intel Corporation 6 Series/C200 Series Chipset Family PCI Express Root Port 1 (rev b5) (prog-if 00 [Normal decode])
    Flags: bus master, fast devsel, latency 0, IRQ 25
    Bus: primary=00, secondary=02, subordinate=02, sec-latency=0
    I/O behind bridge: 0000d000-0000dfff
    Prefetchable memory behind bridge: 00000000f2100000-00000000f21fffff
    Capabilities: <access denied>
    Kernel driver in use: pcieport

00:1c.1 PCI bridge: Intel Corporation 6 Series/C200 Series Chipset Family PCI Express Root Port 2 (rev b5) (prog-if 00 [Normal decode])
    Flags: bus master, fast devsel, latency 0, IRQ 26
    Bus: primary=00, secondary=03, subordinate=03, sec-latency=0
    Memory behind bridge: f7900000-f79fffff
    Capabilities: <access denied>
    Kernel driver in use: pcieport

00:1c.3 PCI bridge: Intel Corporation 6 Series/C200 Series Chipset Family PCI Express Root Port 4 (rev b5) (prog-if 00 [Normal decode])
    Flags: bus master, fast devsel, latency 0, IRQ 27
    Bus: primary=00, secondary=04, subordinate=04, sec-latency=0
    Memory behind bridge: f7800000-f78fffff
    Capabilities: <access denied>
    Kernel driver in use: pcieport

00:1d.0 USB controller: Intel Corporation 6 Series/C200 Series Chipset Family USB Enhanced Host Controller #1 (rev 05) (prog-if 20 [EHCI])
    Subsystem: ASUSTeK Computer Inc. Device 105c
    Flags: bus master, medium devsel, latency 0, IRQ 23
    Memory at f7a07000 (32-bit, non-prefetchable) [size=1K]
    Capabilities: <access denied>
    Kernel driver in use: ehci-pci

00:1f.0 ISA bridge: Intel Corporation HM65 Express Chipset Family LPC Controller (rev 05)
    Subsystem: ASUSTeK Computer Inc. Device 105c
    Flags: bus master, medium devsel, latency 0
    Capabilities: <access denied>
    Kernel driver in use: lpc_ich

00:1f.2 SATA controller: Intel Corporation 6 Series/C200 Series Chipset Family 6 port SATA AHCI Controller (rev 05) (prog-if 01 [AHCI 1.0])
    Subsystem: ASUSTeK Computer Inc. Device 105c
    Flags: bus master, 66MHz, medium devsel, latency 0, IRQ 34
    I/O ports at f0b0 [size=8]
    I/O ports at f0a0 [size=4]
    I/O ports at f090 [size=8]
    I/O ports at f080 [size=4]
    I/O ports at f060 [size=32]
    Memory at f7a06000 (32-bit, non-prefetchable) [size=2K]
    Capabilities: <access denied>
    Kernel driver in use: ahci

00:1f.3 SMBus: Intel Corporation 6 Series/C200 Series Chipset Family SMBus Controller (rev 05)
    Subsystem: ASUSTeK Computer Inc. Device 105c
    Flags: medium devsel, IRQ 3
    Memory at f7a05000 (64-bit, non-prefetchable) [size=256]
    I/O ports at f040 [size=32]

01:00.0 VGA compatible controller: NVIDIA Corporation GF108M [GeForce GT 540M] (rev a1) (prog-if 00 [VGA controller])
    Subsystem: ASUSTeK Computer Inc. Device 105c
    Flags: bus master, fast devsel, latency 0, IRQ 36
    Memory at f6000000 (32-bit, non-prefetchable) [size=16M]
    Memory at e0000000 (64-bit, prefetchable) [size=256M]
    Memory at f0000000 (64-bit, prefetchable) [size=32M]
    I/O ports at e000 [size=128]
    Expansion ROM at f7000000 [disabled] [size=512K]
    Capabilities: <access denied>
    Kernel driver in use: nouveau

02:00.0 Ethernet controller: Realtek Semiconductor Co., Ltd. RTL8111/8168/8411 PCI Express Gigabit Ethernet Controller (rev 06)
    Subsystem: ASUSTeK Computer Inc. Device 105c
    Flags: bus master, fast devsel, latency 0, IRQ 33
    I/O ports at d000 [size=256]
    Memory at f2104000 (64-bit, prefetchable) [size=4K]
    Memory at f2100000 (64-bit, prefetchable) [size=16K]
    Capabilities: <access denied>
    Kernel driver in use: r8169

03:00.0 Network controller: Qualcomm Atheros AR9285 Wireless Network Adapter (PCI-Express) (rev 01)
    Subsystem: Lite-On Communications Inc Device 6661
    Flags: fast devsel, IRQ 17
    Memory at f7900000 (64-bit, non-prefetchable) [disabled] [size=64K]
    Capabilities: <access denied>
    Kernel driver in use: ath9k

04:00.0 USB controller: NEC Corporation uPD720200 USB 3.0 Host Controller (rev 04) (prog-if 30 [XHCI])
    Subsystem: ASUSTeK Computer Inc. Device 105c
    Flags: bus master, fast devsel, latency 0, IRQ 19
    Memory at f7800000 (64-bit, non-prefetchable) [size=8K]
    Capabilities: <access denied>
    Kernel driver in use: xhci_hcd
  