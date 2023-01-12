# Devices

## Configuring Devices

**Devices** define the types of devices connected to the clients. Devices are the peripherals linked to the clients, e.g., EFT providers, Printers, Scanners, scales, etc.

Each device must be defined with its specific attributes and then linked to the clients.

Prior to configuring devices, get the configuration from the hardware specifications.

The following example shows the configuration of a Scale Device.

1. Browse to Touchpoints/Device Types.  
2. Click **+Add Device**.  
3. In the **Touchpoint ID** field enter the ID of the device.  
4. In the **Description** field enter the name of the device.  
5. From the **Device Types** drop-down list, select the Device Type.  
6. Set the **Controlled by EPS** slider to Yes if this device is controlled by an EPS provider. (Relevant to payment devices only).  
7. Click the **+ Add New**.  
8. Define the Configuration Data, for example:  
    a. In the **Key** field enter DeviceInfoType.  
    b. In the **Value** field enter ScaleInfo.  
    c. In the **Key** field enter DtrEnable.  
    d. In the **Value** field enter False.  
    e. In the **Key** field enter IsOPOSCompliant.  
    f. In the **Value** field enter True.  
    g. In the **Key** field enter IsOptional.  
    h. In the **Value** field enter True.  
    i. In the **Key** field enter LogicalName.  
    j. In the **Value** field enter NCRScale.7878.  
    k. In the **Key** field enter ReadTimeout.  
    l. In the **Value** field enter 500.  
    m. In the **Key** field enter RtsEnable.  
    n. In the **Value** field enter False.  
    o. In the **Key** field enter TimeBetweenErrorsInSeconds.  
    p. In the **Value** field enter 3.  
    q. In the **Key** field enter Timeout.  
    r. In the **Value** field enter 1000.  
    s. In the **Key** field enter Type.  
    t. In the **Value** field enter OposScale.  
    u. In the **Key** field enter WriteTimeout.  
    v. In the **Value** field enter 500.

9. Click **Save**.  
