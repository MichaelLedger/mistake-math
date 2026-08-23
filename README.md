# Math

Public mistake notebook for **Math** (`MichaelLedger/mistake-math`).

This repository stores **sanitized public copies** of student mistakes: erased clip pictures, question and answer text, tags, and a public nickname. It never stores personal notes, original handwriting photos, or device IDs.

## Branches

Each grade is a branch. Pull requests must target the matching grade branch, **not** `main`.

| Band | Branches |
| --- | --- |
| Primary | `primary-1` … `primary-6` |
| Junior | `junior-1` … `junior-3` |
| Senior | `senior-1` … `senior-3` |
| University | `university-1` … `university-4` |
| Master’s | `master-1` … `master-3` |
| Other | `phd`, `other` |

`main` only holds this README so the repository is non-empty (GitHub cannot fork an empty repo).

## Layout on a grade branch

```text
entries/{id}/entry.json
entries/{id}/*.jpg
```

`{id}` is SHA-256 of normalized question text plus question-clip image bytes. A matching folder on any subject repo / grade branch blocks a second upload of the same problem.

## How to contribute

Use the Mistake Notebook app. It opens a pull request into the grade branch. Maintainers should review and merge into that grade branch only.

Protect `main` and every grade branch. Do not commit publisher tokens here.
