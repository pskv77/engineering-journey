# Labs

This directory contains focused hands-on exercises.

Labs are used to practice individual mechanisms, tools and troubleshooting scenarios before they are integrated into larger projects.

## Purpose

A lab should answer one or more practical questions such as:

- Can I perform this task independently?
- Do I understand what the system is doing?
- Can I diagnose a broken configuration?
- Can I explain why the solution works?
- Can I reproduce the result without copying a ready-made guide?

## Labs vs Projects

Labs are focused and relatively small.

Examples:

- implement binary search;
- inspect Linux process signals;
- configure file permissions;
- troubleshoot DNS resolution;
- configure an Nginx reverse proxy;
- experiment with Docker networking;
- investigate a failed service.

Projects are larger and combine multiple skills.

A useful lab may later become part of a project.

## Current areas

The repository currently separates labs into:

- `cs/`
- `python/`
- `linux/`
- `windows/`
- `networks/`
- `security/`
- `docker/`
- `devops/`

Additional areas may be added later when required.

## Recommended lab structure

A lab may contain:

    lab-name/
    ├── README.md
    ├── files/
    ├── scripts/
    ├── configs/
    └── evidence/

Not every lab needs all directories.

## Lab README

Each meaningful lab should document:

- objective;
- starting conditions;
- task;
- constraints;
- commands or code created during the work;
- result;
- problems encountered;
- explanation of why the final solution works.

When troubleshooting is involved, also record:

- symptoms;
- hypotheses;
- evidence;
- changes;
- verification.

## Failure is useful

A lab does not need to succeed on the first attempt.

Failed attempts may be preserved when they provide useful diagnostic or engineering lessons.

The important part is understanding:

- what failed;
- why it failed;
- how the cause was identified;
- what fixed it.

## Security

Do not store real production secrets, credentials or confidential company information in labs.

Use:

- synthetic data;
- test credentials;
- isolated virtual machines;
- intentionally vulnerable training environments where appropriate.

## Git usage

Labs should normally be committed in logical steps.

Examples:

    lab: implement binary search
    lab: reproduce systemd failure
    fix: correct nginx upstream configuration
    docs: document docker networking findings

The purpose is to make Git history reflect the learning process rather than only the final result.
