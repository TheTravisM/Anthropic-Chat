

### Step 1: Check existing OpenCode directories
```powershell
Get-ChildItem "$env:APPDATA\opencode", "$env:LOCALAPPDATA\opencode" -ErrorAction SilentlyContinue
```

### Step 2: Clear OpenCode AppData and LocalAppData caches
```PowerShell

Remove-Item -Path "$env:APPDATA\opencode" -Recurse -Force -ErrorAction SilentlyContinue
Remove-Item -Path "$env:LOCALAPPDATA\opencode" -Recurse -Force -ErrorAction SilentlyContinue
```


### Step 3: Clear OpenCode VS Code extension state
```PowerShell
Remove-Item -Path "$env:USERPROFILE\.vscode\extensions\*opencode*" -Recurse -Force -ErrorAct
```

