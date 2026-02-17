# Disable-Windows-Passkeys-Security-Key-Prompts
disable that annoying qr code and usb thing


This small registry tweak disables Windows 11’s built‑in FIDO2 “passkey” system and removes the Security Key sign‑in provider.
It’s meant for people who don’t use hardware security keys, don’t want passkeys, and are tired of Windows or websites triggering QR‑code login popups.

These changes do not affect normal sign‑in methods like:

Microsoft Authenticator

Password

PIN

Windows Hello (except passkeys)

Xbox / Store sign‑ins

Only the passkey and hardware‑key features are disabled.

What This Fixes
After applying the registry file, you will no longer see:

“Sign in with a passkey” QR‑code popups

Prompts asking you to “use a security key”

Websites automatically triggering Windows Hello passkey dialogs

Windows offering FIDO2 as a login option

If you never owned a hardware key and don’t want passkeys, this removes the noise.

Included Changes
The bundled .reg file does two things:

Disables the Windows FIDO2 Platform Authenticator  
This stops Windows from acting like a hardware key and prevents passkey prompts.

Disables the Security Key Credential Provider  
This removes the “Security Key” option from Windows sign‑in settings.

Both changes are reversible.
