## IGCSE O LEVEL COMPUTER SCIENCE NOTES

---

### Section 1: Computer System

#### 1. Data Representation

- 1 bit represents a binary value of either 0 or 1.
- 8 bits constitute 1 byte.
- Subsequently, 1024 bytes form 1 kilobyte (Kb), 1024 kilobytes form 1 Megabyte (MB), 1024 MB make 1 Gigabyte (GB), and 1024 GB make 1 Terabyte (TB).

#### Conversion among Denary, Binary, and Hexadecimal

- Denary (Decimal) - Base 10.
- Binary - Base 2.
- Hexadecimal - Base 16.

#### Relationships

- Denary to Binary
- Denary to Hexadecimal
- Binary to Denary
- Hexadecimal to Denary
- Binary to Hexadecimal
- Hexadecimal to Binary

#### Benefits:

- Understanding data representation helps in efficient storage and manipulation of information.
- Mastery of conversion techniques facilitates understanding of low-level programming and digital electronics.

#### Drawbacks:

- Initial learning curve may be steep for some learners.
- Complex conversions can be time-consuming without practice.

---

### Example 1: Converting 102 Denary to Binary

```less
// Labels of powers of 2 for binary:
128 64 32 16 8 4 2 1 ~ Label

// Placement of denary number under respective labels:
128 64 32 16 8 4 2 1 ~ Label
 0  1  1  0  0 1 1 0

// Analysis:
102 - 128 = ❌
102 - 64 = 38
38 - 32 = 6
// Skipping 16 and 8 as they exceed the target.
6 - 4 = 2
2 - 2 = 0

Result for 102 Denary is: 01100110 in binary.
```

#### Example 2: Converting 01100110 Binary to Denary

```less
// Labels of powers of 2 for binary:
128 64 32 16 8 4 2 1 ~ Label

// Binary values under respective labels:
128 64 32 16 8 4 2 1 ~ Label
 0  1  1  0  0 1 1 0

// Sum of labels with value 1:
64 + 32 + 4 + 2 = 102

Result for 01100110 Binary is: 102 Denary.
```

#### Exercises

1. Convert 302 Denary to Binary step by step.
2. Convert 1011011 Binary to Denary step by step.
3. Convert 204 Denary to Hexadecimal step by step.
4. Convert 11000101 Binary to Hexadecimal step by step.

---

### Representation of Sound

- Sound is analog and needs to be converted to digital for computer processing using ADC (Analog to Digital Converter).

#### Benefits:

- Digital representation enables precise manipulation and storage of sound.
- Facilitates various digital audio processing techniques like compression, filtering, and synthesis.

#### Drawbacks:

- Loss of some detail during analog-to-digital conversion can impact sound quality.
- Higher sampling rates and resolutions lead to larger file sizes.

### Pixel (px)

- Pixel depth varies based on color representation: 1 bit for black and white, 2 bits for four colors, and 3 bits for eight colors.

#### Calculation of file size

- For images: `image resolution (in pixels) × colour depth (in bits)`
- For mono sound files: `sample rate (in Hz) × sample resolution (in bits) × length of sample (in seconds)`

#### Example 1: Calculating Memory Stick Capacity

```
Given: Photograph size is 1024 × 1080 pixels with a color depth of 32 bits.
Memory stick capacity: 64GiB

Calculations:
= (1024 * 1080) * 32
= 1,105,920 * 32
= 35,389,440 bits

Converting bits to bytes:
= 35,389,440 / 8
= 4,423,680 bytes

Memory stick capacity in bytes:
= 64 * 1024 * 1024 * 1024
= 68,719,476,736 bytes

Number of photographs fitting onto the memory stick:
= 68,719,476,736 / 4,423,680
= 15,534.45925925926 photos
```

### Data Compression

#### Reasons for Compression:

- To save storage space
- To enhance transmission speed over networks
- To lower bandwidth consumption
- To reduce our file size.
- To time taken to stream a music.
- To reduce the time taken to upload, download or transfer a file across a network.
- To reduces costs when uploading to cloud.

#### Lossy vs. Lossless Compression

##### Lossy Compression

- File compression algorithm is used
- Eliminates unnecessary data from the file
- Data can't be reconstructed once it has been compressed.
- Results in some loss of detail when compared to the original file.
- Lossy files are more smaller than lossless files.
- Examples include MP3, MP4, and JPEG formats

##### Lossless Compression

- File compression algorithm is used
- All the data from the original uncompressed file can be
  reconstructed / Preserves all original data
- Suitable for situations requiring exact data reconstruction
- It is a form of lossless/reversible file compression
- Reduces the size of a string of adjacent, identical data
- Examples include ZIP and PNG formats
