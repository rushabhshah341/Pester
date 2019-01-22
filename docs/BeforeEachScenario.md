---
external help file: Pester-help.xml
Module Name: Pester
online version:
schema: 2.0.0
---

# BeforeEachScenario

## SYNOPSIS
Defines a ScriptBlock hook to run before each scenario to set up the test environment

## SYNTAX

### All (Default)
```
BeforeEachScenario [-Script] <ScriptBlock> [<CommonParameters>]
```

### Tags
```
BeforeEachScenario [-Tags] <String[]> [-Script] <ScriptBlock> [<CommonParameters>]
```

## DESCRIPTION
BeforeEachScenario hooks are run before each scenario that is in (or above) the folder where the hook is defined.

You should not normally need this, because it overlaps significantly with the "Background" feature in the gherkin language.

This is a convenience method, provided because unlike traditional RSpec Pester,
there is not a simple test script where you can put setup and clean up.

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -Tags
Optional tags.
If set, this hook only runs for features with matching tags

```yaml
Type: System.String[]
Parameter Sets: Tags
Aliases:

Required: True
Position: 1
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -Script
The ScriptBlock to run for the hook

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable.
For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[AfterEachFeature](AfterEachFeature.md)

[AfterEachScenario](AfterEachScenario.md)

[BeforeEachScenario](BeforeEachScenario.md)