================================================
TrendMicro DeepSecurity Collection Release Notes
================================================

.. contents:: Topics


v2.1.0
======

Minor Changes
-------------

- To add unit test case for deepsec_anti_malwares module
- To add unit test case for deepsec_firewall_rules module
- To add unit test case for deepsec_integrity_monitoring_rules, deepsec_intrusion_prevention_rules, and deepsec_log_inspection_rules module

Bugfixes
--------

- To fix the Log inspection rules module bug, where log_files param was not parsed as expected in idempotent play output.

Documentation Changes
---------------------

- Lint documentation and examples.
- To add run output to the docs of all of the existing TM deepsec resource modules.

v2.0.0
======

Major Changes
-------------

- Minimum required ansible.netcommon version is 2.5.1.
- Updated base plugin references to ansible.netcommon.

Documentation Changes
---------------------

- Update module doc

v1.2.0
======

Minor Changes
-------------

- Add AntiMalware rules resource module.
- Add Firewall rules resource module.
- Add Log Inspection rules resource module.
- Add new Integrity Monitoring rules module (https://github.com/ansible-collections/trendmicro.deepsec/pull/24).
- Add new RM states to Intrusion prevention rules module (https://github.com/ansible-collections/trendmicro.deepsec/pull/25).

Documentation Changes
---------------------

- To update comments to get included TM collection under Ansible (https://github.com/ansible-collections/ansible-inclusion/discussions/27#discussioncomment-1016085).

New Modules
-----------

- deepsec_anti_malwares - Manages AntiMalware Rule resource module
- deepsec_firewall_rules - Manages Firewall Rule resource module
- deepsec_integrity_monitoring_rules - Manages Integrity Monitoring Rule resource module
- deepsec_intrusion_prevention_rules - Intrusion Prevention Rule resource module.
- deepsec_log_inspection_rules - Manages Log Inspection Rule resource module

v1.1.0
======

Minor Changes
-------------

- Add deepsec_apikey config module.
- Add deepsec_system_settings config module.

New Modules
-----------

- deepsec_apikey - Create a new and manage API Keys.
- deepsec_system_settings - Modify the system settings for TrendMicro Deep Security.

v1.0.0
======

Minor Changes
-------------

- Add deepsec_anti_malware config module.
- Add deepsec_firewallrules config module.
- Add deepsec_hosts_info config module.
- Add deepsec_log_inspectionrules module.
- Add deepsec_syslog module.

Bugfixes
--------

- Fix no log issues for private_key for deepsec_syslog_config module.

New Modules
-----------

- deepsec_anti_malware - Create a new antimalware under TrendMicro Deep Security Policy
- deepsec_firewallrules - Create a new firewall rule.
- deepsec_hosts_info - Obtain information about one or many Hosts defined by TrendMicro Deep Security
- deepsec_log_inspectionrules - Create a new log inspection rule.
