# Update-ModuleManifest
Aktualisiert eine Modulmanifestdatei

## Beschreibung

Das Cmdlet „Update-ModuleManifest“ aktualisiert eine Modulmanifestdatei (.psd1).

### Hinweise
    - DscResourcesToExport is only supported on the latest PowerShell version 5.0. We won’t be able to update the field if you are running on lower versions of PowerShell.

## Cmdlet-Syntax
```powershell
Get-Command -Name Update-ModuleManifest -Module PowerShellGet -Syntax
```

## Cmdlet-Onlinehilfe

[Update-ModuleManifest](http://go.microsoft.com/fwlink/?LinkId=619311)

## Beispiele für Befehle

Dieses neue Cmdlet wird verwendet, um die Manifestdatei mit eingegebenen Eigenschaftswerten zu aktualisieren. Es verwendet dieselben Parameter wie „New-ModuleManifest“.

Wir stellen fest, dass viele Modulentwickler in exportierten Werten wie „FunctionsToExport“, „CmdletsToExport“ usw. „\*“ angeben möchten. Während der Veröffentlichung des Moduls im PowerShell-Katalog werden nicht angegebene Funktionen und Befehle nicht ordnungsgemäß im Katalog aufgefüllt. Deshalb sollten Modulentwickler ihre Manifeste mit ordnungsgemäßen Werten aktualisieren.

Wenn es Module mit exportierten Eigenschaften gibt, füllt „Update-ModuleManifest“ die angegebene Manifestdatei mit Informationen aus exportierten Funktionen, Cmdlets, Variablen usw. auf:
```powershell
Get-Content -Path "C:\Temp\PSGTEST-TestPackageMetadata\2.5\PSGTEST-TestPackageMetadata.psd1"
@{
# Script module or binary module file associated with this manifest.
# RootModule = ''
# Version number of this module.
ModuleVersion = '2.5'
# ID used to uniquely identify this module
GUID = '610e5c5b-dc42-4eaa-8511-ebfb44066d5e'

#(Other properties removed here for Simplicity…)

# Functions to export from this module
FunctionsToExport = '*'
# Cmdlets to export from this module
CmdletsToExport = '*'
# Variables to export from this module
VariablesToExport = '*'
# Aliases to export from this module
AliasesToExport = '*'
}
```

Nach „Update-ModuleManifest“:
```powershell
Update-ModuleManifest -Path "C:\Temp\PSGTEST-TestPackageMetadata\2.5\PSGTEST-TestPackageMetadata.psd1"
Get-Content -Path "C:\Temp\PSGTEST-TestPackageMetadata\2.5\PSGTEST-TestPackageMetadata.psd1"
#
# Module manifest for module 'NewManifest'
#
# Generated by: author name
#
# Generated on: 11/13/2015
#
@{
# Script module or binary module file associated with this manifest.
# RootModule = ''
# Version number of this module.
ModuleVersion = '2.5'
# ID used to uniquely identify this module
GUID = '610e5c5b-dc42-4eaa-8511-ebfb44066d5e'
# Functions to export from this module
FunctionsToExport = 'Get-FooFn Get-FooWF'
# Cmdlets to export from this module
CmdletsToExport = 'Test-PSGetTestCmdlet'
}
```

Jedem Modul sind auch Metadatenfelder zugeordnet. Um die Metadaten im PowerShell-Katalog ordnungsgemäß anzuzeigen, können Sie mit „Update-ModuleManifest“ diese Felder unter „PrivateData“ auffüllen.

```powershell
Update-ModuleManifest -Path "C:\Temp\PSGTEST-TestPackageMetadata\2.5\PSGTEST-TestPackageMetadata.psd1" -Tags "Tag1" -LicenseUri "http://license.com" -ProjectUri "http://project.com" -IconUri "http://icon.com" -ReleaseNotes "Test module"
```

Die Hashtabelle „PrivateData“ in der Vorlage der Manifestdatei hat die folgenden Eigenschaften

```powershell
# Private data to pass to the module specified in RootModule/ModuleToProcess. This may also contain a PSData hashtable with additional module metadata used by PowerShell.
PrivateData = @{
    PSData = @{
        # Tags applied to this module. These help with module discovery in online galleries.
        # Tags = @()

        # A URL to the license for this module.
        # LicenseUri = ''
    
        # A URL to the main website for this project.
        # ProjectUri = ''
        
        # A URL to an icon representing this module.
        # IconUri = ''
        
        # ReleaseNotes of this module
        # ReleaseNotes = ''
        
        # External dependent modules of this module
        # ExternalModuleDependencies = ''
    } # End of PSData hashtable
} # End of PrivateData hashtable
```



<!--HONumber=Aug16_HO3-->

