# psPAS Changelog


## 1.2.3 (April 17 2018)

- Bug Fixes:
  - `New-PASSession`, `New-PASSAMLSession` & `New-PASSharedSession`
  prevented from providing output (except error message) in the
  event of a failure

## 1.2.0 (March 16 2018)

### Module updated to cover CyberArk 10.2 API features

- New Functions
  - `New-PASOnboardingRule` has added parameters available from 10.2 onwards.
    The 9.8 & 10.2 parameters are configured as separate parametersets.
  - `Get-PASOnboardingRule` has a new parameter added, allowing search of
     Onboarding rules by name in version 10.2
  - `Import-PASPlatform` function added, allowing import of CPM Platforms
  - `Get-PASPSMConnectionParameters` updated to facilitate return of HTML5
      connection data when PSMGW is configured.
  - `Suspend-PASPSMSession` & `Resume-PASPSMSession` functions added, expanding
     on the automatic mitigation capability for PSM Sessions.

- Attained 100% Code Coverage in the Tests for the module.

## 1.1.8 (March 09 2018)

- Bug Fixes:
  - ```Add-PASAccountGroupMember``` now sends AccountID with request.
  - ```New-PASAccountGroup``` fixed an incorrect parameter name (_GroupPlatformID_).
  - ```New-PASSAMLSession``` - basic authentication token now sent in request header.
  - ```Get-PASOnboardingRule```, ```New-PASOnboardingRule``` & ```Remove-PASOnboardingRule```,
    parameters updated to allow specification of alternate PVWA application name
    (in-line with the rest of the module's functions).

## 1.0.6 (February 12 2018)

Published to [PowerShell Gallery](http://powershellgallery.com/packages/psPAS)