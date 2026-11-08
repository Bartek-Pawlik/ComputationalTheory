# Computational Theory: SHA-256

Work for the Computational Theory assessment. It walks through the SHA-256 hash algorithm from [FIPS 180-4](https://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.180-4.pdf) in Python, building up its parts one problem at a time.

Everything is in `problems.ipynb`, with one section per problem. Each section explains the idea, implements it in Python, tests it, and links to the sources it is based on.

## Problems

| Problem | Topic |
| --- | --- |
| 1 | Representing SHA-256 data in Python covering 32-bit words, messages, blocks, the final hash and big-endian integers. |
| 2 | The six SHA-256 bitwise functions (`Ch`, `Maj`, `Sigma0`, `Sigma1`, `sigma0`, `sigma1`), using NumPy 32-bit unsigned integers. |
| 3 | Generating the 64 SHA-256 round constants from the cube roots of the first 64 primes, and checking them against the standard. |

## Repository contents

| File | Description |
| --- | --- |
| `problems.ipynb` | The notebook with all the problems. |
| `requirements.txt` | The Python packages needed to run the notebook. |
| `.gitignore` | Files Git should not track, such as caches and virtual environments. |
| `AGENTS.md` | Guidance for AI assistants used during the assessment. |

## Requirements

- [Python 3](https://www.python.org/downloads/) (developed with Python 3.14)
- [Git](https://git-scm.com/downloads)
- The packages in `requirements.txt`: `jupyter` and `numpy`

## Setup

```bash
git clone https://github.com/Bartek-Pawlik/ComputationalTheory.git
cd ComputationalTheory
pip install -r requirements.txt
```

## Running

```bash
jupyter notebook problems.ipynb
```

Then choose **Kernel → Restart Kernel and Run All Cells**. You can also open the notebook in VS Code with the Jupyter extension.

The tests are `assert` statements inside the notebook, so a full run with no errors means every test passed. The whole notebook runs in a few seconds.

## References

- National Institute of Standards and Technology (2015). [FIPS 180-4: Secure Hash Standard](https://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.180-4.pdf). The official definition of SHA-256.
- [NumPy documentation](https://numpy.org/doc/stable/).
- [Python documentation](https://docs.python.org/3/).

More specific references are given throughout the notebook, next to the parts they support.