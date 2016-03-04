# Introduction
**sr2** is a symbol ranking compressor designed for high speed rather than good compression, developed by **Matt Mahoney**.
**sr3** is a modified version of **sr2**, with a better compression and a slower speed, improved by **Nania Francesco Antonio**.
This program is based on **sr3a**, an enhanced version of **sr3** by **Andre Paterson**.

# Usage
Warning! Input file name will **not** be reserved after compression.
## Compression
sr3 c input output
## Decompression
sr3 d input output

# Simple Benchmark
CPU: Intel® Core™ i5-2520M CPU @ 2.50GHz

File: ReactOS.vdi

| **Method** | **Size** | **Time** | **Compression Rate** |
|-----------------|---------------------|------------------|-------------------|
| `-` | 313524224B | - | 100% |
| `bzip2 -9` | 121913111B | 34.194s | 38.88% |
| `gzip -9` | 128797634B | 34.552s | 41.08% |
| `sr3` | 125657740B | 24.817s | 40.08% |
