# AMU mathematics projects

Undergraduate mathematics work from Ave Maria University, maintained by [27kms](https://github.com/27kms).

## Buffon's needle problem

What is the probability that a needle dropped onto a ruled surface crosses a line? This senior seminar paper studies that question and its connection to estimating pi.

**[Read the paper](Math_Senior_Seminar/Paper.pdf)**

K. M. Sullivan · December 12, 2017 · 11 pages

The paper covers:

- Barbier's solution for short needles using linearity of expectation.
- Calculus solutions for short and long needles.
- Monte Carlo estimation of pi using the short-needle result.

## Repository contents

| File | Contents |
| --- | --- |
| [Paper](Math_Senior_Seminar/Paper.pdf) | Original PDF, preserved unchanged |
| [Archive notes](docs/archive-notes.md) | Provenance, scope, and validation |
| [Source manifest](docs/source-manifest.json) | Original filenames and SHA-256 hashes |
| [Original overview](docs/original-readme.md) | Preserved README from the download |

The download contains the paper only. Its LaTeX source and executable simulation code are not included.

With Python 3.11 or newer already installed, check the preserved files:

```sh
python3 scripts/check_archive.py
```

Related archive: [Penn projects](https://github.com/27kms/penn-projects).
