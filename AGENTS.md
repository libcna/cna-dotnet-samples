AI must not be used to generate code for contributions to this project.

"AI" in this case means a Large Language Model ("LLM"), such as ChatGPT,
Claude, Copilot, Grok, etc.

AI-generated code is based upon sources of unknown origins and may not be 
compatible with the licenses applicable to this project, or may introduce 
conflicting license terms if it includes code from other projects.

AI can be used to identify issues with contributions to this project, but the
solutions to those issues should be authored by humans.

We have found that AI will frequently hallucinate issues that are not actually
problems in practice, report incorrect information, and describe problems that
are actually not issues at all. If AI identifies a problem with this codebase,
please make sure you understand what it is saying and have independently
confirmed that the issue exists before submitting a bug report or pull request.

By submitting a pull request to this project, you confirm that you are the
author of your changes, have the necessary rights to contribute them, and
comply with all applicable licensing requirements of this project.

# CNA.NET Samples Agent Instructions

Before doing any work in this repository, read [`rules.md`](rules.md) completely and obey it. That
applies to analysis, enabling a sample, builds, runs, documentation, commits and reviews.

Read [`plan.md`](plan.md) and the affected sample's `missing.md` as well.

The one thing to understand before touching anything: **this repository does not port samples.**
The original Microsoft C# is checked in as close to verbatim as .NET 8 allows, and everything
needed to build it lives in the project file. A character changed in a `.cs` file is a deviation
that must be recorded; a setting added to `samples/Directory.Build.props` is free.

A defect is fixed where it lives -- `../cna-dotnet`, `../cna` or `../sharp-runtime` -- with a
regression test there, and the same sample is then finished (see `rules.md`). The campaign plan and
ledger is `../cna-dotnet/CAMPAIGN.md`.

Start with [`NEXT.md`](NEXT.md)'s **Active handoff**: it names the row to work on next, the
synchronized head of every repository in the chain, and what the last session left open.
