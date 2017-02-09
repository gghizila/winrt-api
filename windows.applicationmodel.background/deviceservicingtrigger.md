---
-api-type: winrt class
---
 More detail on the policy requirements of the [DeviceServicingTrigger](deviceservicingtrigger.md) background task can be found in the  section of this page.
 For info about using the [DeviceServicingTrigger](deviceservicingtrigger.md), see [Device sync and update for Windows Store device apps](http://go.microsoft.com/fwlink/p/?LinkId=306619 ).
 For info about using the [DeviceUseTrigger](deviceusetrigger.md), see [Accessing sensors and devices from a background task](http://msdn.microsoft.com/library/ccde8565-8dae-44fc-aded-3a0fee759930).
 The [DeviceServicingTrigger](deviceservicingtrigger_deviceservicingtrigger.md) background task requires user consent every time it's triggered.
 Your device must be connected or paired with the PC and available when requesting the [DeviceServicingTrigger](deviceservicingtrigger_deviceservicingtrigger.md).
 Your app is allowed a maximum of 30 minutes (wall clock) of background activity for device updates with [DeviceServicingTrigger](deviceservicingtrigger_deviceservicingtrigger.md)
 Your app is not allowed to request a [DeviceServicingTrigger](deviceservicingtrigger_deviceservicingtrigger.md) background task while your app is not in the foreground.
 Your app can only run one [DeviceServicingTrigger](deviceservicingtrigger_deviceservicingtrigger.md) at a time. Attempting to create a second [DeviceServicingTrigger](deviceservicingtrigger_deviceservicingtrigger.md) will raise an exception.
 The PC's battery must have more than 33% capacity remaining, or the PC must be on A/C power.
 [DeviceServicingTrigger](deviceservicingtrigger_deviceservicingtrigger.md) background tasks may be canceled by Windows when these policy requirements are no longer met, including a maximum amount of wall clock background time.