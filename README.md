# RottenPotato
## Local Privilege Escalation from Windows Service Accounts to SYSTEM

For a technical overview of this exploit see our blog post at https://foxglovesecurity.com/2016/09/26/rotten-potato-privilege-escalation-from-service-accounts-to-system/

### Usage:
1. Compile.
2. Use ILMerge to combine Potato.exe, SharpCifs.dll NHttp.dll, and Microsoft.VisualStudio.OLE.Interop.dll. This will produce a single, portable binary.
3. Get a meterpreter shell on the target system
4. use incognito
5. Run the binary from step.2
6. impersonate_token "NT AUTHORITY\\SYSTEM"

See videos at https://www.youtube.com/watch?v=3CPdKMeB0UY and https://www.youtube.com/watch?v=wK0r-TZR7w8 for example.


