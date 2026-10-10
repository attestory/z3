# Why attestory holds this fork

This is a fork of [Z3Prover/z3](https://github.com/Z3Prover/z3), taken on
2026-09-17 by [attestory](https://github.com/attestory). Upstream is the
source; this file is the only attestory-authored file in the tree.

**Context.** This fork pins Z3 for the symbolic admissible-history work
described below and gives attestory a place for a local patch if one is ever
needed. It is governed by hand, with no ruleset; its ledger is upstream git
history.

**The reason.** attestory builds evidence-first governed delivery: a system
whose state is a set of admissible histories that evidence narrows. Deciding
what is still admissible is a symbolic problem, and Z3 is the solver we
expect to integrate directly into that core rather than call as an external
binary. Holding a fork lets a build pin one exact revision, and carry a local
patch if one is ever needed, instead of depending on a moving upstream
release.

**What this fork is not.** It carries no attestory changes today and no
claim of maintenance. Bugs, questions and patches for Z3 belong upstream at
Z3Prover/z3, not here. The Z3 licence (MIT) and upstream's copyright are
unchanged; nothing in this fork relicences upstream's work.

**Provenance.** The reason above was drafted by the attestory steward and
confirmed by the operator; the organisation's own map of repositories is
private.
