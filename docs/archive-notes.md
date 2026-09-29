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

## Preservation contract

`scripts/approved-imports.json` fixes the reviewed source paths, destination paths, original hashes, imported hashes, and sizes. It was established by comparing the import with the downloaded files. The checker requires the manifest to match this independent baseline and imported bytes to match the approved hashes. Editing the manifest alone cannot authorize an archive change.

These are preserved snapshots. Any change to an imported notebook, including restoring a redacted value in any syntax or location, fails its hash check. Additional notebooks are rejected, including case variants of `.ipynb`. Local `.git`, `.venv`, `venv`, and `.ipynb_checkpoints` directories are excluded. Documentation and maintenance scripts may still be edited.

The checker does not assess arbitrary notebook content for secrets. An intentional future archive revision requires a separately reviewed baseline update and a fresh content review. The baseline is a repository invariant, not protection against someone deliberately changing both the baseline and validator.
