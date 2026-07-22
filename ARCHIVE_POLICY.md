# Archive policy

This organization mirrors the public archives of the R project's mailing lists. This page explains where the content comes from, what we can change, and how to ask for something to be removed.

## Where the content comes from

Every archive repository here is a mirror of a public Mailman pipermail archive. Nothing is collected from private mail, and nothing is reconstructed from any source other than the published archive.

- Most lists are published by ETH Zurich, which indexes them at [stat.ethz.ch/mailman/listinfo](https://stat.ethz.ch/mailman/listinfo). An individual archive lives at a URL like [stat.ethz.ch/pipermail/r-help/](https://stat.ethz.ch/pipermail/r-help/), and the exact upstream URL for a list is recorded in that list's repository README.
- Rcpp-devel is published by [R-Forge](https://lists.r-forge.r-project.org/pipermail/rcpp-devel/).

Each repository keeps the mbox files exactly as upstream publishes them, which means monthly for some lists, quarterly for others, and annually for a few, plus a structured form produced by [rmail-parser](https://github.com/r-mailing-lists/rmail-parser). The [data](https://github.com/r-mailing-lists/data) repository publishes the same messages as Parquet, and the site at [r-mailing-lists.thecoatlessprofessor.com](https://r-mailing-lists.thecoatlessprofessor.com/) reads from that data.

Email addresses appear in the same obfuscated form the upstream archive publishes, for example `name at example.com`. We do not de-obfuscate them, and we do not add addresses that upstream withheld.

## What we can change

We can correct or remove content in this mirror and in the site built from it. If a message is misthreaded, misdated, attributed to the wrong person, or garbled by the parser, that is a bug and we want to hear about it. File it at [r-mailing-lists/feedback](https://github.com/r-mailing-lists/feedback/issues/new/choose).

## What removal does not do

Removal here is removal from this mirror only. It does not reach:

- the upstream archive at stat.ethz.ch or R-Forge, which goes on publishing the message,
- the other public mirrors and search indexes that copy those same archives,
- the inboxes of everyone who received the message when it was sent, or
- copies already downloaded from the Parquet releases.

Two further limits are ours rather than someone else's, and we would rather state them than have you discover them:

- Earlier commits in this mirror's own git history still contain the message after it is removed from the current files. Rewriting that history is possible and we will do it on request, but it does not happen automatically.
- A message in the archive period that is still filling up can be restored by the next daily fetch from upstream. We re-apply the removal once that period closes.

We say this plainly because it matters. If your goal is for a message to stop being findable on the internet, a request here is one step of several, and the upstream archive is the one that matters most. We will point you at the upstream contact if that is what you need.

## Requesting removal

Send removal and privacy requests to [support@caffeinatedmath.com](mailto:support@caffeinatedmath.com). Please do not open a public issue, because an issue would republish the very thing you are asking to have taken down.

Include what you can:

- the list, for example `r-help`,
- the message URL on the site, or the message ID, or the archive month and the subject line,
- what you want removed, whether that is a whole message, a quoted block, or an email address, and
- enough for us to see that the request comes from the message's author, or from the person the content is about.

We read these and we reply. This project is maintained by one person, so please allow a little time.

## Scope

This policy covers the repositories in this organization and the site built from them. It describes how this project operates. It is not legal advice, and it does not try to resolve questions that turn on your jurisdiction.
