---
-api-id: T:Windows.Networking.NetworkOperators.MobileBroadbandAccountWatcherStatus
-api-type: winrt enum
---

<!-- Enumeration syntax
public enum Windows.Networking.NetworkOperators.MobileBroadbandAccountWatcherStatus : int
-->

# MobileBroadbandAccountWatcherStatus

## -description
Describes different states of a [MobileBroadbandAccountWatcherStatus](mobilebroadbandaccountwatcherstatus.md) object.

> [!NOTE]
> This functionality is only available to mobile operator apps and Windows Store app given privileged access by mobile network operators.

For permission to use this API, please reach out to [Network Operators API Permissions](mailto:netopperm@microsoft.com).

For technical help with this API, please reach out to [Network Operators API Help](mailto:netophelp@microsoft.com)

## -enum-fields
### -field Created:0
The watcher has been created but not started and is in its initial state.

### -field Started:1
The watcher has been started and has yet to enumerate the existing accounts.

### -field EnumerationCompleted:2
The watcher is running and has finished enumerating the existing accounts.

### -field Stopped:3
The watcher has been stopped. No events will be delivered while the watcher is in this state.

### -field Aborted:4
The watcher has aborted its watching operation due to an unexpected error condition. No events will be delivered while the watcher is in this state.


## -remarks

## -examples

## -see-also