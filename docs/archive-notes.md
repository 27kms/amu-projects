# Archive notes

This repository was prepared on September 28, 2026 from the `AMU_Projects-main` download. It uses a fresh Git history owned by `27kms`.

The 11-page paper, *Buffon's Needle Problem*, is preserved byte for byte at `Math_Senior_Seminar/Paper.pdf`. It is dated December 12, 2017. The original README is preserved at `docs/original-readme.md`.

The download does not contain LaTeX source, simulation code, or additional projects. The new overview describes only the surviving paper.

## Integrity checks

`docs/source-manifest.json` records the SHA-256 hash and size of each imported file. `.gitattributes` disables automatic line-ending conversion so checkouts preserve these bytes.

Run `python3 scripts/check_archive.py` with an existing Python 3.11 or newer installation. The check verifies the fixed two-file inventory, imported file hashes, provenance descriptions, and local documentation links without installing packages.

Run the synthetic regression tests with `python3 -m unittest discover -s scripts -p 'test_*.py'`. The GitHub Actions workflow runs both commands using tools already present on its runner.

## Credits and reuse

Git commits for this import are attributed to `27kms`. The paper retains its original author name and citations. No additional license is assigned by this import.

## Validation scope

The checker compares manifest source and destination paths with an independent fixed inventory in the script. It verifies imported bytes against the manifest and checks that change descriptions agree with its source and imported hashes. The manifest records provenance; it is not an independent authentication of the original files.

All repository notebooks, including additions outside the import manifest, receive structure checks and checks for eight-digit values following a student-ID label and nonempty `grader_api_key` values. Local `.git`, `.venv`, and `venv` directories are excluded. Grading-key fields must be empty or use `null`, `None`, or `~`; runtime expressions are not supported in this static archive. These checks cover the known assignment fields, not every possible secret format.
