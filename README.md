pagerduty-alert-volume
======================

A quick command-line to get the incident volume assigned to an escalation policy broken down by week. I built this to track if my team's paging volume was getting systemically worse over time.

usage: alert_volume.py [-h] [-e [ESCALATION_POLICY]] A S

Graph alert volumes for a given escalation policy.

positional arguments:
  A                     an API key for PagerDuty
  S                     subdomain for the account

optional arguments:
  -h, --help            show this help message and exit
  -e [ESCALATION_POLICY], --escalation_policy [ESCALATION_POLICY]

If escalation policy is not present, this will list escalation policies and their ids (at least the first 100. Didn't bother to paginate this part).
