# Southern Class 313 announcements

Audio files from the Southern Class 313 on-train announcement system.

## Structure

All audio files, with their original names, are found in the [Original](./Original/) directory.

| Path                                       | Contents                                                    |
| ------------------------------------------ | ----------------------------------------------------------- |
| `Original/`                                | Phrases, chimes, sirens and other standalone announcements  |
| `Original/stations/high/` (`sta_xxx`)      | Station names, high inflection                              |
| `Original/stations/low/` (`stb_xxx`)       | Station names, low inflection                               |
| `Transcripts/`                             | Transcription CSVs, one per folder above                    |

Station files are named with the station's [CRS code](https://www.nationalrail.co.uk/) as the last three letters, e.g. `sta_btn` is Brighton.

## Transcripts

CSVs in [Transcripts](./Transcripts/) use the format produced by [announcement-utils](https://github.com/Rail-Announcements/announcement-utils)
(`id`, `script`, `inflection`, `comment`, `type`, `suppress`).

- Station names come from a lookup of the CRS code in each file name.
- Everything else was transcribed with Whisper large-v2 (voice-activity detection on). Clips with no speech, such as chimes, sirens and silent delay files, are left blank.
- Transcripts are machine-generated and have not been fully proofread.
