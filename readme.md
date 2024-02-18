# IGCSE O LEVEL COMPUTER SCIENCE NOTES

---

## Section 1: Computer System

### 1. Data Representation

- 1 bit = 0 or 1
- 8 bits = 1 byte
- 1024 bytes = 1 kilobyte (Kb)
- 1024 kilobytes = 1 Megabyte (MB)
- 1024 MB = 1 Gigabyte (GB)
- 1024 GB = 1 Terabyte (TB)

#### Conversion between Denary, Binary, and Hexadecimal

- Denary (Decimal) - Base 10 unit
- Binary - Base 2 unit
- Hexadecimal - Base 16 unit

#### Relationships

- Denary to Binary
- Denary to Hexadecimal
- Binary to Denary
- Hexadecimal to Denary
- Binary to Hexadecimal
- Hexadecimal to Binary

---

### Example 1: Converting 102 Denary to Binary

```
// Step 1: Write labels of powers of 2 for binary (powers of 16 for hexadecimal)
128 64 32 16 8 4 2 1 ~ Label

// Step 2: Place the denary number under the label less than the target (102). Equation: target - label

128 64 32 16 8 4 2 1 ~ Label
 0  1  1  0  0 1 1 0

// Analysis:
// 102 - 128 = ❌
// 102 - 64 = 38
// 38 - 32 = 6
// Skipping 16 and 8 as they're greater than our target.
// 6 - 4 = 2
// 2 - 2 = 0

Answer for 102 Denary is: 01100110 in binary.
```

### Example 2: Converting 01100110 Binary to Denary

```
// Step 1: Write labels of powers of 2 for binary (powers of 16 for hexadecimal)
128 64 32 16 8 4 2 1 ~ Label

// Step 2: Place the binary value under all labels
128 64 32 16 8 4 2 1 ~ Label
 0  1  1  0  0 1 1 0

// Step 3: Sum all labels with a value of 1
64 + 32 + 4 + 2 = 102

Answer for 01100110 Binary is: 102 Denary.
```

### Exercises

1. Convert 302 Denary to Binary step by step.
2. Convert 1011011 Binary to Denary step by step.
3. Convert 204 Denary to Hexadecimal step by step.
4. Convert 11000101 Binary to Hexadecimal step by step.

---

## Representation of Sound

- Sound is analog (not electric).
- Computers can't process sound directly.
- Sound must be converted to digital using ADC (Analog to Digital Converter).

## Pixel (px)

- Black and white has 1 bit per px (2^0 = 1).
- Four colors have 2 bits per px (2^2 = 4).
- Eight colors have 3 bits per px (2^3 = 8).

### Calculation of file size

- File size of image is calculated using this equation:

```less
image resolution (in pixels) × colour depth (in bits)
```

- Size of a mono sound file is calculated as:

```less
sample rate (in Hz) × sample resolution (in bits) × length of sample (in seconds)
```

#### Example 1. A photograph is 1024 × 1080 pixels and uses a colour depth of 32 bits. How many photographs of this size would fit onto a memory stick of 64GiB?

```less
= image resolution (in pixels) × colour depth (in bits)
= (1024 * 1080) * 32
= 1,105,920 * 32
= 35,389,440 bits

// 35,389,440 bits to bytes

= 35,389,440 / 8
= 4,423,680 bytes

// 64 GiB to bytes

= 64 * 1024 * 1024 * 1024
= 68,719,476,736 bytes

// find how many pic fit

= 68,719,476,736 / 4,423,680
= 15,534.45925925926 pics

```

### Data compression

reason why we compress our files:

- to save the storage space.
- to reduce our file size.
- to time taken to stream a music.
- to reduce the time taken to upload, download or transfer a file across a network.
- to reduce the bandwidth.
- reduced file size also reduces costs.

### Difference between Lossy and Lossless file compression

#### Lossy

- File compression algorithm is used
- Eliminates unnecessary data from the file
- Data can't be reconstructed once it has been compressed.
- Results in some loss of detail when compared to the original file.
- Lossy files are more smaller than lossless files.

Common lossy file compression algorithms are:
» MPEG-3 (MP3) and MPEG-4 (MP4)
» JPEG.

#### Lossless file compression

- File compression algorithm is used
- all the data from the original uncompressed file can be
  reconstructed
- it is a form of lossless/reversible file compression
- reduces the size of a string of adjacent, identical data
