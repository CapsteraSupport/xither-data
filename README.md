---
license: cc-by-4.0
language:
- en
pretty_name: AI vendor sub-processor notice windows
tags:
- privacy
- gdpr
- dpa
- sub-processors
- vendor-risk
size_categories:
- n<1K
---

# AI vendor sub-processor notice windows

How much notice AI and SaaS vendors say they give before adding a new
sub-processor, quoted from their own data processing agreements, and how often
the pages they publish about customer data change. Published by
[Xither](https://www.xither.com), which keeps dated, hashed copies of those pages.

Exported 2026-09-30. The live, current version is https://www.xither.com/notice-windows.

## Files

**`notice_windows.csv`** (and `.jsonl`): 36 vendors whose DPA states a
notice window we could quote, shortest first.

| Column | Meaning |
|---|---|
| vendor | The vendor's name |
| xither_record | The vendor's page on Xither, with every page we watch and when we read it |
| window, unit | The number the clause states, in calendar or business days |
| quote | The clause, verbatim |
| source_url | The page the quote comes from |
| read_on | The date we read that copy |
| sha256_of_copy | The SHA-256 of the copy we read, so the quote can be checked against it |
| how_found | "read by a person" or "found by pattern" |

**`monthly_changes.csv`**: changes we recorded on the pages we watch, by month
and page type, through 2026-08. We watch 186 vendors. A "recorded"
change is any difference between two readings of a page; "material" is the
subset our rules flag as changing content rather than layout, dates or
navigation.

## What this is not

- **Not every vendor.** A vendor missing from `notice_windows.csv` either states
  no window we could quote or publishes its DPA where we cannot read it. The
  vendor's Xither page says which.
- **Not legal advice.** Each row reports what a page said on the date we read
  it. The quote and the source URL are the finding; read the clause in its
  own document before relying on it.
- **Not current.** Vendors edit these pages. The live version is on the site.

## Citation

Xither, "AI vendor sub-processor notice windows", 2026-09-30, https://www.xither.com/notice-windows
