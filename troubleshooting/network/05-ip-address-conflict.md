# IP Address Conflict

## 1. Problem Description
An IP address conflict occurs when two devices on the same network are assigned the same IP address, causing network connectivity problems.

## 2. Symptoms
- Windows displays an "IP address conflict" notification.
- Network connection disconnects unexpectedly.
- Internet access becomes intermittent.
- The device cannot communicate with other devices on the network.
- Network connectivity is limited or unavailable.

## 3. Possible Causes
- Two devices have been assigned the same static IP address.
- DHCP server configuration issues.
- Incorrect manual IP configuration.
- Router assigning duplicate IP addresses.
- Device reconnecting with outdated network configuration.

## 4. Diagnostic Steps
1. Check the IP address conflict notification.
2. Open Command Prompt.
3. Run `ipconfig` to check the current IP address.
4. Run `ipconfig /all` to review IP address, DHCP status, and network adapter details.
5. Identify whether the affected device uses DHCP or a manually assigned IP address.
6. Check with the network administrator whether another device is using the same IP address.
7. Review the DHCP configuration if authorized.

## 5. Solutions
1. Disconnect and reconnect to the network.
2. Restart the computer if appropriate.
3. If DHCP is enabled, run `ipconfig /release` followed by `ipconfig /renew` to request a new IP address.
4. Verify that manually assigned IP addresses are unique and within the approved network range.
5. Contact the network administrator to investigate DHCP or static IP configuration issues.
6. Avoid changing IP addresses without authorization.

## 6. Verification
- Confirm the device receives a valid IP address.
- Check that the IP address is unique within the network.
- Run `ipconfig` to review the updated configuration.
- Test connectivity using `ping`.
- Verify that internet and network access are restored.

## 7. Prevention
- Use DHCP wherever appropriate.
- Maintain accurate records of statically assigned IP addresses.
- Avoid unauthorized manual IP configuration.
- Monitor DHCP address allocation.
- Report recurring IP conflicts to the network administrator.

## 8. Escalation
Escalate to the network administrator if the IP address conflict persists. Include the affected device details, IP address, DHCP status, error messages, and troubleshooting steps performed.

## 9. Status
Resolved / Unresolved
