# signal-utils

Small MATLAB utilities for unit conversion and signal smoothing.

- `src/` — library functions
- `tests/` — unit tests (MATLAB unit testing framework)

Run the tests locally from the repository root:

```matlab
addpath("src")
results = runtests("tests")
```

CI runs on GitHub Actions — see `.github/workflows/ci.yml`.

On each pull request, CI publishes:

- **Test results**: a "Test Results" check run and a PR comment listing passed/failed tests.
- **Code coverage** for `src/`: a sticky PR comment with line coverage per file (also shown in the run's job summary).
- The raw JUnit and Cobertura XML files, uploaded as the `test-and-coverage-reports` artifact.

PRs from forks get a read-only token, so they get the job summary and artifact but no PR comments.

See the PR checks and comments for test results and coverage.
