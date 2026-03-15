# Microsoft Edge Configuration

Collection of config options, flags and policies for Microsoft Edge.

Based on [RKNF's Chromium Hardening Guide](https://github.com/RKNF404/chromium-hardening-guide), [TommyTran732's Edge Policies](https://github.com/TommyTran732/Microsoft-Edge-Policies)
and Edge policies set by [HotCakeX' Harden Windows Security](https://github.com/HotCakeX/Harden-Windows-Security).
Tailored to my personal requirements and preferences, as such it is heavily biased.

I prefer to configure Edge via the in browser settings first, then flags and policies. That's why a lot of the `Default*Setting` policies are omitted and
why most policies are set as recommended (if possible), not mandatory.
However, if a setting can't be configured in the browser (e.g. `DiagnosticData` can't be turned of completely in the browser settings, but can be as a policy)
or I can't see myself ever wanting to toggle it (e.g. `ShowMicrosoftRewards`) I will set it as mandatory.

Up to date for `Microsoft Edge Version 146.0.3856.59: March 13, 2026`

## Content

### Policies

Policies are provided as a Windows registry file that sets the policies for the whole machine (i.e. under `HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Edge`).
See [policies.reg](./policies.reg).

Check applied policies from within edge under `edge://policy`.

### Flags

Set flags in the browser under `edge://flags`:
- None so far

### Additional

- Blocking connections to `ntp.msn.com` (the new tab page used in Edge) e.g. via a DNS-block in PiHole or similar forces Edge into loading the offline variant of the new tab page.

## References

- [Microsoft Edge Stable Channel Release Notes](https://learn.microsoft.com/en-us/deployedge/microsoft-edge-relnote-stable-channel)
- [Microsoft Edge Policy Documentation](https://learn.microsoft.com/en-us/deployedge/microsoft-edge-policies)

