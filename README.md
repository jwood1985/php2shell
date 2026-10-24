# PHP2Shell Exposure Dashboards for Dynatrace

Dynatrace dashboards to help you find PHP processes that may be affected by PHP2Shell and spot potential signs of exploitation.

## Background

PHP2Shell is a vulnerability that can allow unauthenticated remote code execution on affected PHP versions. Given how widely PHP is deployed, it's worth knowing where you stand.

Full analysis: https://dynatr.ac/4ePj7ZN

## What's Included

| File | Environment |
|------|-------------|
| `PHP2Shell Exposure Assessment - SaaS.json` | Dynatrace SaaS |
| `PHP2Shell Exposure Assessment - Managed.json` | Dynatrace Managed |

## Usage

1. Download the JSON file that matches your environment.
2. In Dynatrace, go to **Dashboards** and choose **Import** (upload the JSON).
3. Open the imported dashboard and review:
   - PHP processes and versions running in your environment
   - Processes that may be vulnerable
   - Potential signs of exploitation
4. Prioritize patching for any affected hosts.

## Requirements

- A Dynatrace SaaS or Managed environment
- OneAgent deployed on the hosts you want to assess
- Permission to import dashboards

## Disclaimer

These dashboards are provided as-is to help with assessment. They do not replace patching, a full security review, or your incident response process.

## Resources

- [Dynatrace blog analysis](https://dynatr.ac/4ePj7ZN)
