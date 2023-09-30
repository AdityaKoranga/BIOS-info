# BIOS Settings and Descriptions

## Processor Configuration

| Setting                          | Value                  | Description |
|----------------------------------|------------------------|-------------|
| Hyper-Threading                  | Disable                | Allows multiple threads to run on each core, improving multitasking. |
| Cores Enabled                    | 0                      | Number of CPU cores enabled. |
| Monitor/Mwait                    | Enable                 | Allows the CPU to wait for events without using power. |
| Execute Disable Bit              | Enable                 | Prevents certain types of malicious buffer overflow attacks. |
| Intel Virtualization Technology  | Enable                 | Enhances virtualization features, improving performance of virtual machines. |
| PPIN Control                     | Unlock/Enable          | Protects processor package information. |
| Hardware Prefetcher              | Enable                 | Predictively loads data into cache to improve performance. |
| Adjacent Cache Prefetch          | Enable                 | Prefetches data for adjacent cache lines. |
| DCU Streamer Prefetcher          | Enable                 | Directs data stream prefetch. |
| DCU IP Prefetcher                | Enable                 | Directs instruction pointer prefetch. |
| LLC Prefetch                     | Disable                | Last Level Cache prefetching. |
| Extended APIC                    | Disable                | Advanced Programmable Interrupt Controller for handling interrupts. |
| AES-NI                           | Enable                 | Accelerates encryption and decryption using the Advanced Encryption Standard. |

## CPU P State Control

| Setting             | Value      | Description |
|---------------------|------------|-------------|
| SpeedStep (Pstates) | Enable     | Adjusts the voltage and core frequency dynamically, improving performance and energy efficiency. |
| Config TDP          | Normal     | Configurable Thermal Design Power. |
| EIST PSD Function   | HW_ALL     | Energy-efficient performance states. |
| Turbo Mode          | Enable     | Allows CPU cores to run faster than the base frequency. |

## Memory Configuration

| Setting                                      | Value      | Description |
|----------------------------------------------|------------|-------------|
| Enhanced PPR Operation Mode                  | Disable    | Predictive Failure Analysis for memory. |
| Operation mode                               | Test and Repair | Memory operation mode. |
| Enforce POR                                  | POR        | Power-on reset settings. |
| PPR Type                                     | Hard PPR   | Predictive Failure Analysis type. |
| Memory Frequency                             | 2933       | Speed at which the memory operates. |
| Data Scrambling for DDR4                     | Auto       | Randomizes data to prevent data patterns. |
| tCCD_L Relaxation                            | Auto       | Adjusts timing parameter for memory. |
| tRWSR Relaxation                             | Disable    | Adjusts read-to-write timing parameter. |
| tRFC Optimization for 16Gb Based DIMM        | Disable    | Adjusts timing for 16Gb memory modules. |
| Refresh Watermarks                           | Auto       | Memory refresh rates. |
| ADR Patrol Scrub Disable                     | Disable    | Address patrol scrubbing. |
| Enable ADR                                   | Enable     | Asynchronous DRAM Refresh. |
| Data Scrambling for NVMDIMM                  | Auto       | Data scrambling for Non-Volatile Memory modules. |
| Erase-Arm NVDIMMS                            | Enable     | Prepares NVDIMM for erasure. |
| Restore NVDIMMS                              | Enable     | Restores data to NVDIMM. |
| Interleave NVDIMMS                           | Disable    | Combines memory addresses for NVDIMMs. |
| Reset Trigger ADR                            | Disable    | ADR trigger on reset. |
| S5 Trigger ADR                               | Disable    | ADR trigger on S5 power state. |
| 2x Refresh Enable                            | Auto       | Doubles memory refresh rate. |

## Memory RAS Configuration

| Setting                         | Value    | Description |
|---------------------------------|----------|-------------|
| Static Virtual Lockstep Mode    | Disable  | Memory mirroring for redundancy. |
| UEFI ARM Mirror                 | Disable  | UEFI memory mirroring. |
| Memory Rank Sparing             | Disable  | Replaces failed memory ranks with spare ranks. |
| Correctable Error Threshold     | 512      | Threshold for correctable memory errors. |
| Intel Run Sure                  | Enable   | Enhances system reliability. |
| SDDC Plus One                   | Disable  | Single Device Data Correction. |
| ADDDC Sparing                   | Disable  | Advanced Double Device Data Correction. |
| Patrol Scrub                    | Enable   | Regularly checks memory for errors. |
| Patrol Scrub Interval           | 24       | Time interval for patrol scrubbing. |


Processor Configuration:
Hyper-Threading [ALL]: This setting allows multiple threads to run on each core of the processor. Disabling it means each core will run only one thread.

Cores Enabled: Specifies the number of CPU cores that are enabled. Setting it to 0 typically means all cores are disabled.

Monitor/Mwait: Enables or disables the MONITOR and MWAIT instructions. These instructions are primarily used for better power management.

Execute Disable Bit: A security feature that can prevent certain types of malicious buffer overflow attacks when combined with a supporting operating system.

Intel Virtualization Technology: Enables or disables hardware virtualization. This is useful for running virtual machines.

PPIN Control: Allows unlocking or enabling the Processor Physical Identification Number.

Hardware Prefetcher: This setting allows the processor to fetch instructions ahead of time to improve performance.

Adjacent Cache Prefetch: Enables the prefetching of cache lines that are adjacent to a cache line that is used.

DCU Streamer Prefetcher & DCU IP Prefetcher: These settings control different types of data cache unit prefetching.

LLC Prefetch: Controls the Last Level Cache prefetching.

Extended APIC: Extended Advanced Programmable Interrupt Controller, used for handling interrupts.

AES-NI: Enables or disables the Advanced Encryption Standard Instruction Set.

CPU P state control:
SpeedStep (Pstates): Allows the processor to adjust its speed to conserve power.

Config TDP: Configurable Thermal Design Power. It defines the power the cooling system is required to dissipate.

EIST PSD Function: Energy-efficient performance states.

Turbo Mode: Allows the processor to run faster than its base operating frequency.

Memory configuration:
Enhanced PPR Operation Mode: Controls the Pseudo Page Rank operation mode.

Operation mode: Determines how the memory operates.

Enforce POR: Power-on reset enforcement.

PPR Type: Pseudo Page Rank type.

Memory Frequency: Specifies the operating frequency of the memory.

Data Scrambling for DDR4 & NVMDIMM: Provides an additional level of data security by constantly changing the data pattern as it is written to the memory.

tCCD_L Relaxation, tRWSR Relaxation, tRFC Optimization for 16Gb Based DIMM: These are advanced memory timing settings.

Refresh Watermarks: Controls when the memory is refreshed.

ADR Patrol Scrub Disable: Controls the Address Range Scrub feature.

Enable ADR: Enables the Asynchronous DRAM Refresh.

Erase-Arm NVDIMMS, Restore NVDIMMS, Interleave NVDIMMS: Controls operations related to Non-Volatile DIMMs.

Reset Trigger ADR & S5 Trigger ADR: Controls the conditions under which ADR is triggered.

Memory RAS Configuration:
Static Virtual Lockstep Mode Mirror mode & UEFI ARM Mirror: These settings are related to memory mirroring, which is a redundancy measure for memory.

Memory Rank Sparing: Allows spare memory ranks to replace failed ones.

Correctable Error Threshold: Specifies the threshold for correctable memory errors.

Intel Run Sure: Provides enhanced reliability, availability, and serviceability (RAS) for enterprise applications.

SDDC Plus One, ADDDC Sparing: Advanced memory error correction techniques.

Patrol Scrub: Regularly checks memory for errors.

Patrol Scrub Interval: Specifies how often the patrol scrub occurs.

