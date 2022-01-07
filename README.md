# Log4j Fixer
## Usage - Linux
### Credit to https://github.com/Gitnerd-1/
    ansible-playbook [-i inventory] [-k][-K] log4j-fixer.yml [-e "[PASSPHRASE=yourSecretHere] [remove_class=True]"]
    # Stores log in ~/log4j_fixes.csv
    # Stores copies of the jar files in a zip [Encrypted if you passed PASSPHRASE=yourSecret] in the same folder as the .jar file was located
    # Sets file permissions on any modified jar files back to what they were at the start 

## Usage - Windows 
### Credit to https://hochwald.net/post/powershell-based-log4j-vulnerabilities-scanner/ 
    PS>  .\Find-Log4jVulnerabilities.ps1 [-AutoFix] [-WorkDirectory "X:\Path"] 
    # Stores logs in C:\tmep\log4j-vscan
    # Stores a copy of the modified jar files in "saved_files.out" (it's a zip file just renamed) in $WorkDirectory (Defaults to C:\temp\log4j-vscan) 
