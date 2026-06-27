# Submission History

This archive does not vendor the raw submission ZIP files, but the local Downloads history shows a clear iteration sequence from `submission1.zip` through `submission15.zip`, followed by a final `submission.zip`.

## Recorded Sequence

- `submission1.zip` — 2026-03-21 20:08
- `submission2.zip` — 2026-03-22 14:28
- `submission3.zip` — 2026-03-24 15:39
- `submission4.zip` — 2026-03-24 17:55
- `submission5.zip` — 2026-03-24 20:11
- `submission6.zip` — 2026-03-24 21:34
- `submission7.zip` — 2026-03-25 13:19
- `submission8.zip` — 2026-03-25 19:28
- `submission9.zip` — 2026-03-25 20:25
- `submission10.zip` — 2026-03-25 21:04
- `submission11.zip` — 2026-03-25 21:25
- `submission12.zip` — 2026-03-26 13:56
- `submission13.zip` — 2026-03-26 14:47
- `submission14.zip` — 2026-03-26 21:17
- `submission15.zip` — 2026-03-26 21:53
- `submission.zip` — 2026-03-27 11:16

## What The ZIPs Contain

Each sampled ZIP appears to contain the same packaging shape:

- `adapter_model.safetensors`
- `adapter_config.json`

## What The Sequence Suggests

- There was sustained late-stage iteration across March 24 to March 27.
- The file size shifts imply multiple adapter revisions rather than a single unchanged repack.
- The final `submission.zip` appears to be the end-state package after the numbered sequence.

## Why The ZIPs Are Not In Git

The ZIPs are large binary payloads, mostly weight artifacts, and would add noise and storage cost to the archive repository without being diff-friendly. Their existence and cadence are preserved here instead.

## If You Want A Deeper Historical Record Later

Useful follow-up work would be:

1. extract the `adapter_config.json` from each submission ZIP and compare them
2. record any score or leaderboard change associated with each submission
3. keep a separate off-git cloud folder with the raw ZIPs if full preservation matters