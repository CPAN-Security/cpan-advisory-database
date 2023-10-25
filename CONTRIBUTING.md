## Contributing

All work is done on `triage/`.

If you are *reviewing an unpublished report*, make sure all information
regarding said report is filled and correct, then add an extra
`'approved: true'` statement to the document. If the report is invalid, delete
it and, if it has a CVE number, add it to the 'false\_positives' file
with a short explanation on why it is a false positive. You may use the
`cpansec-admin triage` command to make the entire review process smoother
and less error prone. At the end, submit the changes as as a Pull Request.

If you are adding a new report, please either name it as its CVE code or,
in its absence, the CPAN distribution's name. If the name clashes with
another file currently under triage, append a number (like a timestamp)
to the end of the file name. Do not add the 'approved: true' statement.
Then create a PR with your new file.

Once your PR is reviewed and merged to the repository, a robot will run
and publish it for you, assigning a proper CPANSEC-ID.

Thank you for your contribution!
