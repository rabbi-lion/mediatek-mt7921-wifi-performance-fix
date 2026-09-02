````markdown
# MediaTek MT7921 Wi-Fi Performance Fix

A troubleshooting guide for poor Wi-Fi performance and connection stability with the MediaTek Wi-Fi 6 MT7921 wireless adapter on Windows.

Some systems using the MT7921 may experience problems such as:

- unusually low download or upload speeds
- inconsistent Wi-Fi performance
- high latency or latency spikes
- intermittent connection problems
- instability when using Wi-Fi 6

These problems can also be caused by drivers, signal quality, interference or router configuration, so the settings below should be treated as troubleshooting steps rather than a universal fix.

## Update the Wi-Fi Driver

Before changing adapter settings, check whether a newer Wi-Fi driver is available from your laptop or motherboard manufacturer.

For laptops in particular, prefer the driver provided by the system manufacturer when one is available.

You can check the currently installed driver through:

```text
Device Manager → Network adapters → MediaTek Wi-Fi 6 MT7921 Wireless LAN Card → Properties → Driver
```

If the problem started after a driver update, testing an older manufacturer-provided driver may also help.

## Open the Adapter Settings

Open:

```text
Device Manager
```

Expand:

```text
Network adapters
```

Right-click:

```text
MediaTek Wi-Fi 6 MT7921 Wireless LAN Card
```

and select:

```text
Properties
```

Open the:

```text
Advanced
```

tab.

The exact property names available here can vary depending on the installed driver and computer manufacturer.

## Disable Wi-Fi 6 for Testing

Find the wireless mode setting.

Depending on the driver, it may be named something similar to:

```text
802.11ax/ac/n/abg
```

Change the value from a mode that includes:

```text
802.11ax
```

to:

```text
802.11ac
```

This disables Wi-Fi 6 for the adapter and makes it use Wi-Fi 5 instead.

Apply the setting and test the connection again.

If performance or stability improves significantly, the problem may be related to the adapter's Wi-Fi 6 operation, driver or interaction with the wireless access point.

## Reduce Roaming Aggressiveness

In the same **Advanced** tab, look for:

```text
Roaming Aggressiveness
```

If the option is available, set it to the lowest available value or disable it if the driver provides a disabled option.

Lower roaming aggressiveness makes the adapter less likely to search for and switch between access points.

This is most useful on a desktop or laptop that normally remains connected to the same wireless access point.

Apply the setting and test the connection again.

## Test the Connection

After changing the settings, reconnect to your Wi-Fi network and test:

- download speed
- upload speed
- latency
- connection stability

Change one setting at a time when troubleshooting so you can determine which change actually improves the connection.

## Restore Wi-Fi 6

If disabling Wi-Fi 6 does not improve the connection, return to:

```text
Device Manager → Network adapters → MediaTek Wi-Fi 6 MT7921 Wireless LAN Card → Properties → Advanced
```

Restore the original wireless mode that includes:

```text
802.11ax
```

You can also restore the original **Roaming Aggressiveness** setting if changing it did not help.

## Additional Troubleshooting

If the problem continues:

1. Install the latest Wi-Fi driver provided by your laptop or motherboard manufacturer.
2. Test another manufacturer-provided driver version if the problem began after an update.
3. Restart the router and computer.
4. Test the computer closer to the wireless access point.
5. Test both 5 GHz and 2.4 GHz networks if both are available.
6. Remove and reconnect to the Wi-Fi network in Windows.
7. Restore the adapter's default Advanced settings if previous changes did not help.

Avoid changing several adapter settings at once, as this makes it difficult to determine which setting affected the problem.

## Notes

Disabling 802.11ax limits the MT7921 to Wi-Fi 5 and therefore disables Wi-Fi 6 features.

This may reduce maximum theoretical wireless throughput, but it can be useful as a troubleshooting step when Wi-Fi 6 operation is unstable.

The exact names and available values of the MT7921 Advanced properties vary between driver versions and computer manufacturers.

Poor Wi-Fi performance is not necessarily caused by the wireless adapter itself. Signal strength, interference, router configuration, router firmware and driver versions can produce similar symptoms.

## References

This guide was written independently using Microsoft Windows troubleshooting information and MediaTek MT7921 troubleshooting reports as technical references.

Relevant documentation:

- Microsoft Windows Wi-Fi troubleshooting documentation
- Microsoft Community and Microsoft Q&A MT7921 troubleshooting information
- Documentation and drivers provided by the computer or motherboard manufacturer

Windows and wireless drivers change over time. Check the current driver and documentation provided by your computer manufacturer before troubleshooting.

## License

Made by rabbi-lion.

Original text in this repository is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License.

Referenced projects, documentation and third-party material retain their respective rights and licenses.

See `LICENSE` for the full license text.
````
