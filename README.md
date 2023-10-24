# The CPAN Advisory Database

This is a community owned repository of advisories for Perl modules and
distributions published on [CPAN](https://metacpan.org).

All advisories are stored as individual JSON files in this repository,
formatted using the [Open Source Vulnerability (OSV) format](https://ossf.github.io/osv-schema/).

It is maintained by the CPAN Security Working Group, under the Perl Toolchain Gang and MetaCPAN.

## Repository Structure

`advisories/`

Folder that stores all published advisories, ready for public consumption.

`triage/`

Folder that stores entries not yet assigned to a CPAN Advisory Id.

`triage/last_visited_index`

Keeps track of the last visited index on NVD, so
[cpansec-admin](https://metacpan.org/pod/CPANSEC::Admin) doesn't
have to re-scan everything when it runs.

`triage/false_positives`

a list of CVE entries that are marked as a false positive by moderation,
meaning they were found by `cpansec-admin` but are not - nor have ever been -
on CPAN. Those will be ignored by `cpansec-admin` when it runs.


