# Technology Add-on for Vectra Cognito

**Author:** Vectra Networks

**Version:**

* @version@

**Supported products:**

* Vectra X Series

**Supported CIM Version:**

* &gt;=4.0.0

**Supported CIM Datamodels:**

* Intrusion Detection

**Sourcetypes:**

* `vectra:cognito:audit`
* `vectra:cognito:campaigns`
* `vectra:cognito:cef`
* `vectra:cognito:detect`
* `vectra:cognito:health`
* `vectra:cognito:hostscoring`

**Add-on contains:**

* Search and Parsing-Time configuration

**Input requirements:**

* This release requires Vectra X series to send data in syslog CEF format

## Using this Technology Add-on

* The add-on has to be installed on Search Heads
* If data is collected through Intermediate Heavy Forwarders, it has to be installed on Heavy Forwarders, otherwise on indexers
* The add-on expects an initial sourcetype named `vectra:cognito:cef`, the sourcetype will be transformed into more specific ones (see sourcetype list)
* A sample `inputs.conf` is provided (`default/inputs.conf.sample`)

## Compatibility

* The Vectra App For Splunk is currently not compatible with this Technology Add-on.
* Data previously indexed with sourcetype `Vectra-CEF` can be added to the intrusion detection datamodel, by renaming the sourcetype to  `vectra:cognito:detect`.
Following stanza needs to be added in e.g. `$SPLUNK_HOME/apps/TA-vectra-cognito/props.conf`:

```ini
[Vectra-CEF]
rename = vectra:cognito:detect
```

## Release Notes

* **1.0.0 / 2018-11-29** mbo

  * Initial Release

* **1.0.1 / 2018-03-09** mbo

  * Bugfix Release

## Change Log

* **1.0.0 / 2018-11-29** mbo

  * Initial Release
  
* **1.0.1 / 2019-03-09** mbo

  * Typo in field naming