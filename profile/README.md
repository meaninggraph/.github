# MeaningGraph

**Shared, reusable meanings for data.**

A column called `Country`, `BillingCountry` or `cntry_code` means the same thing in a
thousand databases, and every tool, analyst and AI agent works that out again from scratch.
MeaningGraph writes such meanings down once, as small open files, so that people and
software can reuse them: what a *country*, an *invoice* or a *sale* is, what it is also
called, how it is measured, and which fields of a particular dataset carry it.

## Watch

<a href="https://youtu.be/FQKSkWI0qDM"><img src="https://meaninggraph.io/images/intro-film-poster.jpg" alt="MeaningGraph.I/O — What a number means: watch the intro film (1:43)" width="560"></a>

▶ **[What a number means — the MeaningGraph.I/O intro film (1:43)](https://youtu.be/FQKSkWI0qDM)**

## How it fits together

- **Universal concepts** (country, currency and money, invoice, customer, population,
  *per capita* and more) live in this organisation and are versioned like code.
- **A dataset's meaning file** extends and refers to those concepts, and binds them to its
  own fields, which are described in [ModelSpec](https://github.com/specscore/modelspec),
  an open, storage-neutral data model language.
- **Tools read both.** A query tool or an AI agent can then answer "which countries buy
  the most?" knowing which field means *country*, which means *sale*, and how to compare
  them fairly.

## Used in DataTug development

[DataTug](https://datatug.app) is working on connecting its model structure to shared meanings in this graph, alongside ModelSpec. The semantic integration is ongoing. [Explore the tools behind DataTug](https://datatug.app/en/under-the-hood/tools-we-built/#contracts).

The first worked example is being written for the
[Chinook sample database](https://github.com/datatug/chinookdb) (chinookdb.com).

## Status

Early. The file format is a first draft and will change. The first repository of
universal concepts is [meaninggraph/core](https://github.com/meaninggraph/core).
Registered graphs are listed in [meaninggraph/registry](https://github.com/meaninggraph/registry),
an inGitDB database checked on every change.

## Links

- Website: [meaninggraph.io](https://meaninggraph.io)
- Universal concepts: [meaninggraph/core](https://github.com/meaninggraph/core)
- Registry: [meaninggraph/registry](https://github.com/meaninggraph/registry)
- ModelSpec: [github.com/specscore/modelspec](https://github.com/specscore/modelspec)
