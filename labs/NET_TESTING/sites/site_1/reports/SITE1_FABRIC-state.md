# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed | Total Tests Skipped |
| ----------- | ------------------ | ------------------ | ------------------- |
| 414 | 374 | 8 | 32 |

### Summary Totals Device Under Test

| Device Under Test | Total Tests | Tests Passed | Tests Failed | Tests Skipped | Categories Failed | Categories Skipped |
| ------------------| ----------- | ------------ | ------------ | ------------- | ----------------- | ------------------ |
| s1-brdr1 | 55 | 50 | 1 | 4 | System | Hardware |
| s1-brdr2 | 55 | 50 | 1 | 4 | System | Hardware |
| s1-leaf1 | 56 | 51 | 1 | 4 | System | Hardware |
| s1-leaf2 | 56 | 51 | 1 | 4 | System | Hardware |
| s1-leaf3 | 56 | 51 | 1 | 4 | System | Hardware |
| s1-leaf4 | 56 | 51 | 1 | 4 | System | Hardware |
| s1-spine1 | 40 | 35 | 1 | 4 | System | Hardware |
| s1-spine2 | 40 | 35 | 1 | 4 | System | Hardware |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed | Tests Skipped |
| ------------- | ----------- | ------------ | ------------ | ------------- |
| BGP | 54 | 54 | 0 | 0 |
| Connectivity | 108 | 108 | 0 | 0 |
| Hardware | 32 | 0 | 0 | 32 |
| Interfaces | 108 | 108 | 0 | 0 |
| Logging | 16 | 16 | 0 | 0 |
| MLAG | 6 | 6 | 0 | 0 |
| Routing | 74 | 74 | 0 | 0 |
| System | 16 | 8 | 8 | 0 |

## Failed Test Results Summary

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 55 | s1-brdr1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 110 | s1-brdr2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 166 | s1-leaf1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 222 | s1-leaf2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 278 | s1-leaf3 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 334 | s1-leaf4 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 374 | s1-spine1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 414 | s1-spine2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |

## All Test Results

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 1 | s1-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine1 (IP: 10.250.1.1) | PASS | - |
| 2 | s1-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine2 (IP: 10.250.1.2) | PASS | - |
| 3 | s1-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-brdr2 (IP: 10.252.1.9) | PASS | - |
| 4 | s1-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine1 (IP: 172.16.1.16) | PASS | - |
| 5 | s1-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine2 (IP: 172.16.1.18) | PASS | - |
| 6 | s1-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-brdr2 Ethernet1 | PASS | - |
| 7 | s1-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-spine1 Ethernet7 | PASS | - |
| 8 | s1-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-spine2 Ethernet7 | PASS | - |
| 9 | s1-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-brdr2 Ethernet6 | PASS | - |
| 10 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-brdr1 Loopback0 (IP: 10.250.1.7) | PASS | - |
| 11 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-brdr2 Loopback0 (IP: 10.250.1.8) | PASS | - |
| 12 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-leaf1 Loopback0 (IP: 10.250.1.3) | PASS | - |
| 13 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-leaf2 Loopback0 (IP: 10.250.1.4) | PASS | - |
| 14 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-leaf3 Loopback0 (IP: 10.250.1.5) | PASS | - |
| 15 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-leaf4 Loopback0 (IP: 10.250.1.6) | PASS | - |
| 16 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-spine1 Loopback0 (IP: 10.250.1.1) | PASS | - |
| 17 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-spine2 Loopback0 (IP: 10.250.1.2) | PASS | - |
| 18 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.17) - Destination: s1-spine1 Ethernet7 (IP: 172.16.1.16) | PASS | - |
| 19 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.19) - Destination: s1-spine2 Ethernet7 (IP: 172.16.1.18) | PASS | - |
| 20 | s1-brdr1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 21 | s1-brdr1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 22 | s1-brdr1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 23 | s1-brdr1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 24 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-brdr2_Ethernet1 = 'up' | PASS | - |
| 25 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-spine1_Ethernet7 = 'up' | PASS | - |
| 26 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-spine2_Ethernet7 = 'up' | PASS | - |
| 27 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - P2P_s2-brdr1_Ethernet4 = 'up' | PASS | - |
| 28 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-brdr2_Ethernet6 = 'up' | PASS | - |
| 29 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 30 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 31 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-brdr2_Port-Channel1 = 'up' | PASS | - |
| 32 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 33 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 34 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan30 - Thiry = 'up' | PASS | - |
| 35 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 36 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 37 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 38 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 39 | s1-brdr1 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 40 | s1-brdr1 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 41 | s1-brdr1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 42 | s1-brdr1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 43 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.1 - Peer: s1-spine1 | PASS | - |
| 44 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.2 - Peer: s1-spine2 | PASS | - |
| 45 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.3 - Peer: s1-leaf1 | PASS | - |
| 46 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.4 - Peer: s1-leaf2 | PASS | - |
| 47 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.5 - Peer: s1-leaf3 | PASS | - |
| 48 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.6 - Peer: s1-leaf4 | PASS | - |
| 49 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.7 - Peer: s1-brdr1 | PASS | - |
| 50 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.8 - Peer: s1-brdr2 | PASS | - |
| 51 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: s1-leaf1 | PASS | - |
| 52 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: s1-leaf3 | PASS | - |
| 53 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.7 - Peer: s1-brdr1 | PASS | - |
| 54 | s1-brdr1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 55 | s1-brdr1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 56 | s1-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine1 (IP: 10.250.1.1) | PASS | - |
| 57 | s1-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine2 (IP: 10.250.1.2) | PASS | - |
| 58 | s1-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-brdr1 (IP: 10.252.1.8) | PASS | - |
| 59 | s1-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine1 (IP: 172.16.1.20) | PASS | - |
| 60 | s1-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine2 (IP: 172.16.1.22) | PASS | - |
| 61 | s1-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-brdr1 Ethernet1 | PASS | - |
| 62 | s1-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-spine1 Ethernet8 | PASS | - |
| 63 | s1-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-spine2 Ethernet8 | PASS | - |
| 64 | s1-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-brdr1 Ethernet6 | PASS | - |
| 65 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-brdr1 Loopback0 (IP: 10.250.1.7) | PASS | - |
| 66 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-brdr2 Loopback0 (IP: 10.250.1.8) | PASS | - |
| 67 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-leaf1 Loopback0 (IP: 10.250.1.3) | PASS | - |
| 68 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-leaf2 Loopback0 (IP: 10.250.1.4) | PASS | - |
| 69 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-leaf3 Loopback0 (IP: 10.250.1.5) | PASS | - |
| 70 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-leaf4 Loopback0 (IP: 10.250.1.6) | PASS | - |
| 71 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-spine1 Loopback0 (IP: 10.250.1.1) | PASS | - |
| 72 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-spine2 Loopback0 (IP: 10.250.1.2) | PASS | - |
| 73 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.21) - Destination: s1-spine1 Ethernet8 (IP: 172.16.1.20) | PASS | - |
| 74 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.23) - Destination: s1-spine2 Ethernet8 (IP: 172.16.1.22) | PASS | - |
| 75 | s1-brdr2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 76 | s1-brdr2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 77 | s1-brdr2 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 78 | s1-brdr2 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 79 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-brdr1_Ethernet1 = 'up' | PASS | - |
| 80 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-spine1_Ethernet8 = 'up' | PASS | - |
| 81 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-spine2_Ethernet8 = 'up' | PASS | - |
| 82 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - P2P_s2-brdr2_Ethernet5 = 'up' | PASS | - |
| 83 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-brdr1_Ethernet6 = 'up' | PASS | - |
| 84 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 85 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 86 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-brdr1_Port-Channel1 = 'up' | PASS | - |
| 87 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 88 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 89 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan30 - Thiry = 'up' | PASS | - |
| 90 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 91 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 92 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 93 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 94 | s1-brdr2 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 95 | s1-brdr2 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 96 | s1-brdr2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 97 | s1-brdr2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 98 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.1 - Peer: s1-spine1 | PASS | - |
| 99 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.2 - Peer: s1-spine2 | PASS | - |
| 100 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.3 - Peer: s1-leaf1 | PASS | - |
| 101 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.4 - Peer: s1-leaf2 | PASS | - |
| 102 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.5 - Peer: s1-leaf3 | PASS | - |
| 103 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.6 - Peer: s1-leaf4 | PASS | - |
| 104 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.7 - Peer: s1-brdr1 | PASS | - |
| 105 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.8 - Peer: s1-brdr2 | PASS | - |
| 106 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: s1-leaf1 | PASS | - |
| 107 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: s1-leaf3 | PASS | - |
| 108 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.7 - Peer: s1-brdr1 | PASS | - |
| 109 | s1-brdr2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 110 | s1-brdr2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 111 | s1-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine1 (IP: 10.250.1.1) | PASS | - |
| 112 | s1-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine2 (IP: 10.250.1.2) | PASS | - |
| 113 | s1-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf2 (IP: 10.252.1.1) | PASS | - |
| 114 | s1-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine1 (IP: 172.16.1.0) | PASS | - |
| 115 | s1-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine2 (IP: 172.16.1.2) | PASS | - |
| 116 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-leaf2 Ethernet1 | PASS | - |
| 117 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-spine1 Ethernet2 | PASS | - |
| 118 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-spine2 Ethernet2 | PASS | - |
| 119 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-leaf2 Ethernet6 | PASS | - |
| 120 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-brdr1 Loopback0 (IP: 10.250.1.7) | PASS | - |
| 121 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-brdr2 Loopback0 (IP: 10.250.1.8) | PASS | - |
| 122 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-leaf1 Loopback0 (IP: 10.250.1.3) | PASS | - |
| 123 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-leaf2 Loopback0 (IP: 10.250.1.4) | PASS | - |
| 124 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-leaf3 Loopback0 (IP: 10.250.1.5) | PASS | - |
| 125 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-leaf4 Loopback0 (IP: 10.250.1.6) | PASS | - |
| 126 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-spine1 Loopback0 (IP: 10.250.1.1) | PASS | - |
| 127 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-spine2 Loopback0 (IP: 10.250.1.2) | PASS | - |
| 128 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.1) - Destination: s1-spine1 Ethernet2 (IP: 172.16.1.0) | PASS | - |
| 129 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.3) - Destination: s1-spine2 Ethernet2 (IP: 172.16.1.2) | PASS | - |
| 130 | s1-leaf1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 131 | s1-leaf1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 132 | s1-leaf1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 133 | s1-leaf1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 134 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-leaf2_Ethernet1 = 'up' | PASS | - |
| 135 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-spine1_Ethernet2 = 'up' | PASS | - |
| 136 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-spine2_Ethernet2 = 'up' | PASS | - |
| 137 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - SERVER_s1-host1_eth1 = 'up' | PASS | - |
| 138 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-leaf2_Ethernet6 = 'up' | PASS | - |
| 139 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 140 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 141 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-leaf2_Port-Channel1 = 'up' | PASS | - |
| 142 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - SERVER_s1-host1 = 'up' | PASS | - |
| 143 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 144 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 145 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan30 - Thiry = 'up' | PASS | - |
| 146 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 147 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 148 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 149 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 150 | s1-leaf1 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 151 | s1-leaf1 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 152 | s1-leaf1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 153 | s1-leaf1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 154 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.1 - Peer: s1-spine1 | PASS | - |
| 155 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.2 - Peer: s1-spine2 | PASS | - |
| 156 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.3 - Peer: s1-leaf1 | PASS | - |
| 157 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.4 - Peer: s1-leaf2 | PASS | - |
| 158 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.5 - Peer: s1-leaf3 | PASS | - |
| 159 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.6 - Peer: s1-leaf4 | PASS | - |
| 160 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.7 - Peer: s1-brdr1 | PASS | - |
| 161 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.8 - Peer: s1-brdr2 | PASS | - |
| 162 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: s1-leaf1 | PASS | - |
| 163 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: s1-leaf3 | PASS | - |
| 164 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.7 - Peer: s1-brdr1 | PASS | - |
| 165 | s1-leaf1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 166 | s1-leaf1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 167 | s1-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine1 (IP: 10.250.1.1) | PASS | - |
| 168 | s1-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine2 (IP: 10.250.1.2) | PASS | - |
| 169 | s1-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf1 (IP: 10.252.1.0) | PASS | - |
| 170 | s1-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine1 (IP: 172.16.1.4) | PASS | - |
| 171 | s1-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine2 (IP: 172.16.1.6) | PASS | - |
| 172 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-leaf1 Ethernet1 | PASS | - |
| 173 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-spine1 Ethernet3 | PASS | - |
| 174 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-spine2 Ethernet3 | PASS | - |
| 175 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-leaf1 Ethernet6 | PASS | - |
| 176 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-brdr1 Loopback0 (IP: 10.250.1.7) | PASS | - |
| 177 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-brdr2 Loopback0 (IP: 10.250.1.8) | PASS | - |
| 178 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-leaf1 Loopback0 (IP: 10.250.1.3) | PASS | - |
| 179 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-leaf2 Loopback0 (IP: 10.250.1.4) | PASS | - |
| 180 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-leaf3 Loopback0 (IP: 10.250.1.5) | PASS | - |
| 181 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-leaf4 Loopback0 (IP: 10.250.1.6) | PASS | - |
| 182 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-spine1 Loopback0 (IP: 10.250.1.1) | PASS | - |
| 183 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-spine2 Loopback0 (IP: 10.250.1.2) | PASS | - |
| 184 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.5) - Destination: s1-spine1 Ethernet3 (IP: 172.16.1.4) | PASS | - |
| 185 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.7) - Destination: s1-spine2 Ethernet3 (IP: 172.16.1.6) | PASS | - |
| 186 | s1-leaf2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 187 | s1-leaf2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 188 | s1-leaf2 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 189 | s1-leaf2 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 190 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-leaf1_Ethernet1 = 'up' | PASS | - |
| 191 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-spine1_Ethernet3 = 'up' | PASS | - |
| 192 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-spine2_Ethernet3 = 'up' | PASS | - |
| 193 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - SERVER_s1-host1_eth2 = 'up' | PASS | - |
| 194 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-leaf1_Ethernet6 = 'up' | PASS | - |
| 195 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 196 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 197 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-leaf1_Port-Channel1 = 'up' | PASS | - |
| 198 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - SERVER_s1-host1 = 'up' | PASS | - |
| 199 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 200 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 201 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan30 - Thiry = 'up' | PASS | - |
| 202 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 203 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 204 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 205 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 206 | s1-leaf2 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 207 | s1-leaf2 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 208 | s1-leaf2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 209 | s1-leaf2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 210 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.1 - Peer: s1-spine1 | PASS | - |
| 211 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.2 - Peer: s1-spine2 | PASS | - |
| 212 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.3 - Peer: s1-leaf1 | PASS | - |
| 213 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.4 - Peer: s1-leaf2 | PASS | - |
| 214 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.5 - Peer: s1-leaf3 | PASS | - |
| 215 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.6 - Peer: s1-leaf4 | PASS | - |
| 216 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.7 - Peer: s1-brdr1 | PASS | - |
| 217 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.8 - Peer: s1-brdr2 | PASS | - |
| 218 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: s1-leaf1 | PASS | - |
| 219 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: s1-leaf3 | PASS | - |
| 220 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.7 - Peer: s1-brdr1 | PASS | - |
| 221 | s1-leaf2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 222 | s1-leaf2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 223 | s1-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine1 (IP: 10.250.1.1) | PASS | - |
| 224 | s1-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine2 (IP: 10.250.1.2) | PASS | - |
| 225 | s1-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf4 (IP: 10.252.1.5) | PASS | - |
| 226 | s1-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine1 (IP: 172.16.1.8) | PASS | - |
| 227 | s1-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine2 (IP: 172.16.1.10) | PASS | - |
| 228 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-leaf4 Ethernet1 | PASS | - |
| 229 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-spine1 Ethernet4 | PASS | - |
| 230 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-spine2 Ethernet4 | PASS | - |
| 231 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-leaf4 Ethernet6 | PASS | - |
| 232 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-brdr1 Loopback0 (IP: 10.250.1.7) | PASS | - |
| 233 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-brdr2 Loopback0 (IP: 10.250.1.8) | PASS | - |
| 234 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-leaf1 Loopback0 (IP: 10.250.1.3) | PASS | - |
| 235 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-leaf2 Loopback0 (IP: 10.250.1.4) | PASS | - |
| 236 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-leaf3 Loopback0 (IP: 10.250.1.5) | PASS | - |
| 237 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-leaf4 Loopback0 (IP: 10.250.1.6) | PASS | - |
| 238 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-spine1 Loopback0 (IP: 10.250.1.1) | PASS | - |
| 239 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-spine2 Loopback0 (IP: 10.250.1.2) | PASS | - |
| 240 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.9) - Destination: s1-spine1 Ethernet4 (IP: 172.16.1.8) | PASS | - |
| 241 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.11) - Destination: s1-spine2 Ethernet4 (IP: 172.16.1.10) | PASS | - |
| 242 | s1-leaf3 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 243 | s1-leaf3 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 244 | s1-leaf3 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 245 | s1-leaf3 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 246 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-leaf4_Ethernet1 = 'up' | PASS | - |
| 247 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-spine1_Ethernet4 = 'up' | PASS | - |
| 248 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-spine2_Ethernet4 = 'up' | PASS | - |
| 249 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - SERVER_s1-host2_eth1 = 'up' | PASS | - |
| 250 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-leaf4_Ethernet6 = 'up' | PASS | - |
| 251 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 252 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 253 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-leaf4_Port-Channel1 = 'up' | PASS | - |
| 254 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - SERVER_s1-host2 = 'up' | PASS | - |
| 255 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 256 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 257 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan30 - Thiry = 'up' | PASS | - |
| 258 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 259 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 260 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 261 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 262 | s1-leaf3 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 263 | s1-leaf3 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 264 | s1-leaf3 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 265 | s1-leaf3 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 266 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.1 - Peer: s1-spine1 | PASS | - |
| 267 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.2 - Peer: s1-spine2 | PASS | - |
| 268 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.3 - Peer: s1-leaf1 | PASS | - |
| 269 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.4 - Peer: s1-leaf2 | PASS | - |
| 270 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.5 - Peer: s1-leaf3 | PASS | - |
| 271 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.6 - Peer: s1-leaf4 | PASS | - |
| 272 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.7 - Peer: s1-brdr1 | PASS | - |
| 273 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.8 - Peer: s1-brdr2 | PASS | - |
| 274 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: s1-leaf1 | PASS | - |
| 275 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: s1-leaf3 | PASS | - |
| 276 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.7 - Peer: s1-brdr1 | PASS | - |
| 277 | s1-leaf3 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 278 | s1-leaf3 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 279 | s1-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine1 (IP: 10.250.1.1) | PASS | - |
| 280 | s1-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine2 (IP: 10.250.1.2) | PASS | - |
| 281 | s1-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf3 (IP: 10.252.1.4) | PASS | - |
| 282 | s1-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine1 (IP: 172.16.1.12) | PASS | - |
| 283 | s1-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine2 (IP: 172.16.1.14) | PASS | - |
| 284 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-leaf3 Ethernet1 | PASS | - |
| 285 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-spine1 Ethernet5 | PASS | - |
| 286 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-spine2 Ethernet5 | PASS | - |
| 287 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-leaf3 Ethernet6 | PASS | - |
| 288 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-brdr1 Loopback0 (IP: 10.250.1.7) | PASS | - |
| 289 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-brdr2 Loopback0 (IP: 10.250.1.8) | PASS | - |
| 290 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-leaf1 Loopback0 (IP: 10.250.1.3) | PASS | - |
| 291 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-leaf2 Loopback0 (IP: 10.250.1.4) | PASS | - |
| 292 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-leaf3 Loopback0 (IP: 10.250.1.5) | PASS | - |
| 293 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-leaf4 Loopback0 (IP: 10.250.1.6) | PASS | - |
| 294 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-spine1 Loopback0 (IP: 10.250.1.1) | PASS | - |
| 295 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-spine2 Loopback0 (IP: 10.250.1.2) | PASS | - |
| 296 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.13) - Destination: s1-spine1 Ethernet5 (IP: 172.16.1.12) | PASS | - |
| 297 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.15) - Destination: s1-spine2 Ethernet5 (IP: 172.16.1.14) | PASS | - |
| 298 | s1-leaf4 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 299 | s1-leaf4 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 300 | s1-leaf4 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 301 | s1-leaf4 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 302 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-leaf3_Ethernet1 = 'up' | PASS | - |
| 303 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-spine1_Ethernet5 = 'up' | PASS | - |
| 304 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-spine2_Ethernet5 = 'up' | PASS | - |
| 305 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - SERVER_s1-host2_eth2 = 'up' | PASS | - |
| 306 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-leaf3_Ethernet6 = 'up' | PASS | - |
| 307 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 308 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 309 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-leaf3_Port-Channel1 = 'up' | PASS | - |
| 310 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - SERVER_s1-host2 = 'up' | PASS | - |
| 311 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 312 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 313 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan30 - Thiry = 'up' | PASS | - |
| 314 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 315 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 316 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 317 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 318 | s1-leaf4 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 319 | s1-leaf4 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 320 | s1-leaf4 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 321 | s1-leaf4 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 322 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.1 - Peer: s1-spine1 | PASS | - |
| 323 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.2 - Peer: s1-spine2 | PASS | - |
| 324 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.3 - Peer: s1-leaf1 | PASS | - |
| 325 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.4 - Peer: s1-leaf2 | PASS | - |
| 326 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.5 - Peer: s1-leaf3 | PASS | - |
| 327 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.6 - Peer: s1-leaf4 | PASS | - |
| 328 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.7 - Peer: s1-brdr1 | PASS | - |
| 329 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.8 - Peer: s1-brdr2 | PASS | - |
| 330 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: s1-leaf1 | PASS | - |
| 331 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: s1-leaf3 | PASS | - |
| 332 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.7 - Peer: s1-brdr1 | PASS | - |
| 333 | s1-leaf4 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 334 | s1-leaf4 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 335 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-brdr1 (IP: 10.250.1.7) | PASS | - |
| 336 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-brdr2 (IP: 10.250.1.8) | PASS | - |
| 337 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf1 (IP: 10.250.1.3) | PASS | - |
| 338 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf2 (IP: 10.250.1.4) | PASS | - |
| 339 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf3 (IP: 10.250.1.5) | PASS | - |
| 340 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf4 (IP: 10.250.1.6) | PASS | - |
| 341 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-brdr1 (IP: 172.16.1.17) | PASS | - |
| 342 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-brdr2 (IP: 172.16.1.21) | PASS | - |
| 343 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf1 (IP: 172.16.1.1) | PASS | - |
| 344 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf2 (IP: 172.16.1.5) | PASS | - |
| 345 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf3 (IP: 172.16.1.9) | PASS | - |
| 346 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf4 (IP: 172.16.1.13) | PASS | - |
| 347 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-leaf1 Ethernet2 | PASS | - |
| 348 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-leaf2 Ethernet2 | PASS | - |
| 349 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: s1-leaf3 Ethernet2 | PASS | - |
| 350 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: s1-leaf4 Ethernet2 | PASS | - |
| 351 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet7 - Remote: s1-brdr1 Ethernet2 | PASS | - |
| 352 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet8 - Remote: s1-brdr2 Ethernet2 | PASS | - |
| 353 | s1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.0) - Destination: s1-leaf1 Ethernet2 (IP: 172.16.1.1) | PASS | - |
| 354 | s1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.4) - Destination: s1-leaf2 Ethernet2 (IP: 172.16.1.5) | PASS | - |
| 355 | s1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet4 (IP: 172.16.1.8) - Destination: s1-leaf3 Ethernet2 (IP: 172.16.1.9) | PASS | - |
| 356 | s1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet5 (IP: 172.16.1.12) - Destination: s1-leaf4 Ethernet2 (IP: 172.16.1.13) | PASS | - |
| 357 | s1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet7 (IP: 172.16.1.16) - Destination: s1-brdr1 Ethernet2 (IP: 172.16.1.17) | PASS | - |
| 358 | s1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet8 (IP: 172.16.1.20) - Destination: s1-brdr2 Ethernet2 (IP: 172.16.1.21) | PASS | - |
| 359 | s1-spine1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 360 | s1-spine1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 361 | s1-spine1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 362 | s1-spine1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 363 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-leaf1_Ethernet2 = 'up' | PASS | - |
| 364 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-leaf2_Ethernet2 = 'up' | PASS | - |
| 365 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - P2P_s1-leaf3_Ethernet2 = 'up' | PASS | - |
| 366 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - P2P_s1-leaf4_Ethernet2 = 'up' | PASS | - |
| 367 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet7 - P2P_s1-brdr1_Ethernet2 = 'up' | PASS | - |
| 368 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet8 - P2P_s1-brdr2_Ethernet2 = 'up' | PASS | - |
| 369 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 370 | s1-spine1 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 371 | s1-spine1 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 372 | s1-spine1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 373 | s1-spine1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 374 | s1-spine1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 375 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-brdr1 (IP: 10.250.1.7) | PASS | - |
| 376 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-brdr2 (IP: 10.250.1.8) | PASS | - |
| 377 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf1 (IP: 10.250.1.3) | PASS | - |
| 378 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf2 (IP: 10.250.1.4) | PASS | - |
| 379 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf3 (IP: 10.250.1.5) | PASS | - |
| 380 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf4 (IP: 10.250.1.6) | PASS | - |
| 381 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-brdr1 (IP: 172.16.1.19) | PASS | - |
| 382 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-brdr2 (IP: 172.16.1.23) | PASS | - |
| 383 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf1 (IP: 172.16.1.3) | PASS | - |
| 384 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf2 (IP: 172.16.1.7) | PASS | - |
| 385 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf3 (IP: 172.16.1.11) | PASS | - |
| 386 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf4 (IP: 172.16.1.15) | PASS | - |
| 387 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-leaf1 Ethernet3 | PASS | - |
| 388 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-leaf2 Ethernet3 | PASS | - |
| 389 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: s1-leaf3 Ethernet3 | PASS | - |
| 390 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: s1-leaf4 Ethernet3 | PASS | - |
| 391 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet7 - Remote: s1-brdr1 Ethernet3 | PASS | - |
| 392 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet8 - Remote: s1-brdr2 Ethernet3 | PASS | - |
| 393 | s1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.2) - Destination: s1-leaf1 Ethernet3 (IP: 172.16.1.3) | PASS | - |
| 394 | s1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.6) - Destination: s1-leaf2 Ethernet3 (IP: 172.16.1.7) | PASS | - |
| 395 | s1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet4 (IP: 172.16.1.10) - Destination: s1-leaf3 Ethernet3 (IP: 172.16.1.11) | PASS | - |
| 396 | s1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet5 (IP: 172.16.1.14) - Destination: s1-leaf4 Ethernet3 (IP: 172.16.1.15) | PASS | - |
| 397 | s1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet7 (IP: 172.16.1.18) - Destination: s1-brdr1 Ethernet3 (IP: 172.16.1.19) | PASS | - |
| 398 | s1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet8 (IP: 172.16.1.22) - Destination: s1-brdr2 Ethernet3 (IP: 172.16.1.23) | PASS | - |
| 399 | s1-spine2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 400 | s1-spine2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 401 | s1-spine2 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 402 | s1-spine2 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 403 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-leaf1_Ethernet3 = 'up' | PASS | - |
| 404 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-leaf2_Ethernet3 = 'up' | PASS | - |
| 405 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - P2P_s1-leaf3_Ethernet3 = 'up' | PASS | - |
| 406 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - P2P_s1-leaf4_Ethernet3 = 'up' | PASS | - |
| 407 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet7 - P2P_s1-brdr1_Ethernet3 = 'up' | PASS | - |
| 408 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet8 - P2P_s1-brdr2_Ethernet3 = 'up' | PASS | - |
| 409 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 410 | s1-spine2 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 411 | s1-spine2 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 412 | s1-spine2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 413 | s1-spine2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 414 | s1-spine2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
