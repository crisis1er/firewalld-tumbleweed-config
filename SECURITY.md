# Security Policy

## Supported scope
This repository contains firewalld configuration examples, policies, zone definitions, and related documentation for openSUSE Tumbleweed deployments.

Security issues in scope include:
- Unsafe default firewall exposure.
- Incorrect zone, policy, or service definitions that could weaken host protection.
- Configuration mistakes that could break expected filtering behavior.
- Dangerous documentation errors that could lead to insecure deployments.

Out of scope:
- General Linux support questions.
- Distribution packaging issues unrelated to this repository.
- Problems caused only by local environment customizations outside the repository content.

## Reporting a vulnerability
Please report suspected security issues privately first. Include:
- A clear description of the issue.
- The affected file or path.
- Reproduction steps.
- Expected behavior and actual behavior.
- Impact assessment if known.

Do not publish proof-of-concept exploit details before a fix or mitigation is available.

## Response expectations
Reports will be reviewed and triaged as quickly as possible. Valid issues will be acknowledged, assessed, and fixed according to severity and maintenance capacity.

## Hardening note
Because this repository may be used on systems with SELinux, strict firewalling, and production services, proposed changes should favor least privilege and explicit documentation of impact.
