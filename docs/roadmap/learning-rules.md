# Learning Rules

This document defines the operating rules of the engineering learning system.

These rules apply across sprints, labs, projects, assessments and roadmap revisions.

# Rule 1 — Practice dominates theory

The target balance is approximately:

- 20% theory;
- 80% practical work.

Theory should explain mechanisms required for practice.

Watching or reading material without using it is not considered sufficient learning.

# Rule 2 — Skills must be cumulative

Previously learned technologies should continue appearing in future work.

Examples:

- Git is used everywhere;
- Python continues inside Linux;
- Linux continues inside Docker;
- networking continues inside containers;
- Docker continues into CI/CD;
- CI/CD continues into Kubernetes;
- security applies to every stage.

Skills should become interconnected rather than remain isolated topics.

# Rule 3 — Evidence over feeling

Skill ranks are not based only on perceived confidence.

Evidence may include:

- working code;
- configuration;
- labs;
- projects;
- troubleshooting;
- assessment results;
- explanations;
- work experience.

A statement such as "I think I understand it" is not sufficient evidence.

# Rule 4 — Course completion is not skill completion

Courses are learning resources.

A completed course does not automatically increase a skill rank.

Knowledge from courses should be transferred into independent practice.

# Rule 5 — Git is the default working environment

Learning artifacts should normally be stored and developed through Git.

Use:

- branches;
- logical commits;
- pull requests;
- review;
- merge;
- history.

Git itself is part of the engineering practice.

# Rule 6 — Labs and projects have different roles

Labs train focused mechanisms.

Projects combine multiple mechanisms into systems.

Both are required.

Labs should not replace integrated projects.

Projects should not eliminate focused experimentation.

# Rule 7 — Troubleshooting is mandatory

Configuration alone is insufficient.

Important skills must include failure diagnosis.

Preferred process:

    symptom
        ↓
    hypothesis
        ↓
    evidence
        ↓
    diagnosis
        ↓
    change
        ↓
    verification

Broken systems are intentionally useful learning environments.

# Rule 8 — Independence determines rank

Ranks primarily measure the level of independent capability.

Documentation may be allowed for normal engineering tasks.

Step-by-step external solutions should not be required at higher ranks.

# Rule 9 — Unknown answers are acceptable

During assessments, writing:

    не знаю

is better than fabricating an answer.

Unknown answers provide clean diagnostic information.

The goal of assessment is accurate measurement rather than maximizing a score.

# Rule 10 — Confidence is separate from correctness

When appropriate, confidence should be recorded independently.

Confidence scale:

- 0 — guess / unknown;
- 1 — low confidence;
- 2 — medium confidence;
- 3 — high confidence.

Confident incorrect answers may indicate misconceptions.

Correct low-confidence answers may indicate unstable knowledge.

# Rule 11 — Assessment remains strict

Assessment grading should not be softened because:

- a topic was difficult;
- the learner was tired;
- the technology is new;
- progress has otherwise been good.

Context may affect interpretation, but not the correctness of the answer itself.

# Rule 12 — Rechecks are required

Short-term success is not sufficient.

Important topics should normally be checked again after approximately 4–6 weeks.

Older skills should also appear in cumulative assessments.

# Rule 13 — The HomeLab is the primary systems environment

Linux, Windows, networking and infrastructure skills should increasingly be practiced inside the HomeLab.

The environment should evolve with the roadmap.

It should include both normal and intentionally broken scenarios.

# Rule 14 — Security is integrated

Security should not be postponed until the final specialization phase.

Every technology should include security considerations relevant to that technology.

# Rule 15 — Do not rush advanced platforms

Technologies such as Kubernetes and cloud platforms should not be introduced merely because they are popular.

They should be introduced after the underlying mechanisms are sufficiently understood.

# Rule 16 — One evolving system is preferred

Whenever practical, projects should extend an existing system.

Preferred progression:

    simple program
        ↓
    service
        ↓
    database
        ↓
    API
        ↓
    Linux deployment
        ↓
    reverse proxy
        ↓
    containers
        ↓
    CI/CD
        ↓
    monitoring
        ↓
    IaC
        ↓
    Kubernetes
        ↓
    cloud

This creates experience with system evolution rather than disconnected tutorials.

# Rule 17 — Documentation is part of engineering

Important work should explain:

- objective;
- architecture;
- decisions;
- failures;
- fixes;
- verification;
- remaining limitations.

Documentation should reflect actual implementation.

# Rule 18 — Protect sensitive information

Never store real production secrets or confidential company data in the learning repository.

Use synthetic:

- credentials;
- users;
- networks;
- datasets;
- configurations.

# Rule 19 — Sustainable consistency

The normal target workload is approximately 8–10 hours per week.

A difficult week may be reduced to approximately 5–6 hours.

A high-capacity week may reach approximately 10–12 hours.

The system should favor sustainable progress over burnout.

# Rule 20 — The roadmap is allowed to change

Roadmap changes are expected when supported by new evidence.

Valid reasons include:

- assessment results;
- work experience;
- university experience;
- project discoveries;
- professional opportunities;
- changes in interests.

Changes should be documented and versioned.

The objective is not to obey Roadmap v1 forever.

The objective is to continuously improve the learning system.
