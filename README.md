# Technology Add-on for Vectra Cognito

**Author:** Vectra Networks

**Version:**

* @version@

**Supported products:**

* Vectra X Series

**Supported CIM Version:**

* >=4.0.0

**Supported CIM Datamodels:**

* Intrusion Detection

**Source types:**

* vectra:cognito:audit
* vectra:cognito:campaings
* vectra:cognito:cef
* vectra:cognito:detect
* vectra:cognito:health
* vectra:cognito:hostscoring

**Add-on contains:**

* Search and Parsing-Time configuration

**Input requirements:**

* This release requires Vectra X series to send data in syslog CEF format

## Using this Technology Add-on

* The add-on has to be installed on search-heads
* If data is collected through Intermediate Heavy Forwarders, it has to be installed on Heavy Forwarders, otherwise on indexers
* The add-on expects an initial sourcetype named "vectra:cognito:cef", the sourcetype will be transformed into more specific ones
* A sample inputs.conf is provided (default/inputs.conf.sample)

## Compatibility

* This app is not compatible with the Vectra App For Splunk
* For compatibility reasons, all data previously indexed with a sourcetype Vectra-CEF will be renamed into the sourcetype "vectra:cognito:detect"

## Release Notes

* **1.0.0 / 2018-11-29** mbo

  * Initial Release

## Change Log

* **1.0.0 / 2018-11-29** mbo

  * Initial Release