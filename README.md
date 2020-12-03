# Storage Function Library
For the Management of NAV App Storage to store NAV Deployment files From/To Local System and From/To Azure Storage

## Table of Contents

* [Prerequisites](#Prerequisites)
* [Running the tests](#Running the tests)

## Prerequisites:
Must be connected to Audibene Network through LAN, OfficeWIFI, VPN or From Servers

## Running the tests

Below are the examples to Run /Use these Scripts:
1. To Import Module:
Import-Module .\StorageFunctionLibrary.psm1

2. To Download Files from Azure Storage to Local System:
Download-NAVAppStorage -Environment 'prd' -Name 'TestApp2' -Destination 'C:\tmp\download\'
Please Update Environment, Name and Destination according to your Requirement

3. To Upload Files From Local System to Azure Storage
Add-NAVAppStorage -Environment 'testNirmal2FN' -Name 'TestApp2' -Version '1.0.0.11' -Source 'C:\tmp\config.txt'
Add-NAVAppStorage -Environment 'testNirmal2FN' -Name 'TestApp2' -Version '1.0.0.11' -Source 'C:\tmp\app.txt', 'C:\tmp\runtimepackage.txt'
Please Update Environment, name, version and Source according to your requirement
