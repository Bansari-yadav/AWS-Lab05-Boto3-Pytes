# Lab05 submission notes

The README contains the three written answers required by the assignment submission checklist: the Moto paragraph, the error-handling comparison, and the two-sentence Challenge 5 reflection. They were checked against the locally available assignment PDF, especially Parts I and J and the submission checklist on pages 27-29. No SUBMISSION_NOTES.md existed in this checkout before this update.

## Evidence and limits

- The nine checklist screenshots are embedded in the README, with purpose, command, actual result, and explanation. Original images are preserved unchanged in docs/screenshots/.
- The original test counts are 19 unit, 14 integration, and 2 chaos (35 total). This documentation update adds no tests. A new local deliberate-failure experiment and restored passing unit run were performed; AWS deployment, integration, chaos, and cleanup operations were not rerun.
- The recorded 180-second recovery run passed: uploader about 69.42 seconds, viewer about 73.64 seconds. The separate 60-second run failed: uploader about 83.45 seconds, viewer about 80.31 seconds.
- Folder evidence uses the root listing. Cleanup evidence uses the two supplied cleanup captures, A and B. The extra recursive listing, third cleanup capture, and post-cleanup resource-list image are omitted from the submission.
- The selected break-it evidence is now a new browser report screenshot displaying the actual changed source line and failing test output. The complete run is saved in docs/break_it_new_run.txt. It is explicitly labeled as a report view, not a raw terminal/editor capture or the historical run. The temporary mutation caused 1 failed, 18 passed, 16 deselected (23.70 seconds); restoring the original policy byte-for-byte produced 19 passed, 16 deselected (21.73 seconds). The original historical failure image remains preserved but is no longer embedded. The historical final unit-result crop does not show its command; README labels that limitation.
- No supplied evidence confirms Part I step 5's comparison with the Lab04 output file or restoration of the local SLO after the 60-second run. Neither is claimed as verified.
- Part J challenges 1-4 are not completed in the inspected repo. Existing port 3000 checks are not the port 22 drift test, and a working integer conversion is not the requested friendly-error test for "fast".
- Local configuration, virtual environments, AWS credentials, private keys, generated stack outputs, and backups must stay outside Git. Screenshots contain a credentials-file location message, but no credential values were visible in the inspected images.

See [README screenshot evidence](README.md#screenshot-evidence) for the images and commands.

## Submission checklist review

- Folder layout: README screenshot 1 shows the root files and folders; the repository guide and tracked source provide the module layout.
- Unit tests: screenshot 3 shows the original 19-pass run; the new saved output also confirms 19 passes after restoration.
- Break-it experiment: screenshot 2 shows the actual changed source and failure message from a new run. It is a browser report screenshot; if the instructor requires a raw terminal/editor capture specifically, capture that view manually.
- Stack creation: screenshot 4 shows completion and both URLs.
- Integration: screenshot 5 shows all 14 passing.
- Recovery: screenshots 6 and 7 show the 180-second success and separate 60-second failure for both tiers.
- Cleanup: screenshots 8 and 9 show both supplied successful runs.
- Written answers: the Moto paragraph, exception-handling comparison, and two-sentence Challenge 5 reflection are present.
- Part J challenges 1-4 remain unclaimed; this update does not implement them.
