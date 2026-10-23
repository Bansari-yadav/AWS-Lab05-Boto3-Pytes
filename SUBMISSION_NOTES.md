# Lab05 submission notes

The README contains the three written answers required by the assignment submission checklist: the Moto paragraph, the error-handling comparison, and the two-sentence Challenge 5 reflection. They were checked against the locally available assignment PDF, especially Parts I and J and the submission checklist on pages 27-29. No SUBMISSION_NOTES.md existed in this checkout before this update.

## Evidence and limits

- The nine checklist screenshots are embedded in the README, with purpose, command, actual result, and explanation. Original images are preserved unchanged in docs/screenshots/.
- The original test counts are 19 unit, 14 integration, and 2 chaos (35 total). This documentation update adds no tests and does not rerun AWS deployment, integration, chaos, or cleanup operations.
- The recorded 180-second recovery run passed: uploader about 69.42 seconds, viewer about 73.64 seconds. The separate 60-second run failed: uploader about 83.45 seconds, viewer about 80.31 seconds.
- Folder evidence uses the root listing. Cleanup evidence uses the two supplied cleanup captures, A and B. The extra recursive listing, third cleanup capture, and post-cleanup resource-list image are omitted from the submission.
- The break-it screenshot shows the policy assertion and diff, but does not include a separate editor capture of the modified source line. The final unit-result crop does not show its command; README labels that limitation.
- No supplied evidence confirms Part I step 5's comparison with the Lab04 output file or restoration of the local SLO after the 60-second run. Neither is claimed as verified.
- Part J challenges 1-4 are not completed in the inspected repo. Existing port 3000 checks are not the port 22 drift test, and a working integer conversion is not the requested friendly-error test for "fast".
- Local configuration, virtual environments, AWS credentials, private keys, generated stack outputs, and backups must stay outside Git. Screenshots contain a credentials-file location message, but no credential values were visible in the inspected images.

See [README screenshot evidence](README.md#screenshot-evidence) for the images and commands.
