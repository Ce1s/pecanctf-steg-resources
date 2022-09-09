# STEG TOOLS INSTALLED ON THE PROVIDED KALI MACHINE
## AUDACITY
An open-source audio file and waveform-viewing tool. Audio waveforms can be seen using the spectogram view. Audacity can also enable you to slow down, reverse, and do other manipulations that might reveal a hidden message if you suspect there is one (if you can hear garbled audio, interference, or static).

## SONIC VISUALIZER
A program for viewing and analysing the contents of music audio files. Can be better than AUDACITY for spectrogram viewing.

## GIMP
GIMP or other image editing software like Photoshop can be used to uncover the flag by using different filters and colour ranges.

## EXIFTOOL
Sometimes important stuff is hidden in the metadata of the image or the file. EXIFTOOL can be very helpful to view the metadata of the files.

Useful commands:

```exiftool file``` shows the metadata of the given file.

## STEGHIDE
STEGHIDE is a steganography program that hides data in various kinds of image and audio files. It only supports these file formats: JPEG, BMP, WAV and AU. It’s also useful for extracting embedded and encrypted data from other files.

Useful commands:

```steghide info file``` displays info about a file whether it has embedded data or not.

```steghide extract -sf file``` extracts embedded data from a file.

## STEGSOLVE
Sometimes there is a message or text hidden in the image itself and in order to view it you need to apply some colour filters or play with the colour levels. You can do it with GIMP or Photoshop or any other image editing software but STEGSOLVE makes it easier.

## STRINGS
STRINGS is a Linux tool that displays printable strings in a file. This simple tool can be very helpful when solving steg challenges. The embedded data can be password protected or encrypted. Sometimes the password is actually in the file itself and can be easily viewed by using strings. It’s a default Linux tool.

Useful commands:

```strings file``` displays printable strings in the given file.

## BINWALK
BINWALK is a tool for searching binary files like images and audio files for embedded files and data.

Useful commands:

```binwalk file``` displays the embedded data in the given file.

```binwalk -e file``` displays and extracts the data from the given file.

## ZSTEG
ZSTEG is a tool that can detect hidden data in PNG and BMP files.

Useful commands:

```zsteg -a file``` runs all the methods on the given file.

```zsteg -E file``` extracts data from the given payload.

## LSB_STEG_DECODE.PY
Python program based on steganographic methods to hide files in images using the Least Significant Bit technique. More details at: https://github.com/RobinDavid/LSB-Steganography

## PYTHON STEGANO LIBRARY
A Python programming language library which can be imported into scripts to solve steganography challenges.


# Guides and lists of tools for steganography CTF challenges
https://medium.com/@FourOctets/ctf-tidbits-part-1-steganography-ea76cc526b40
https://project-awesome.org/apsdehal/awesome-ctf#steganography-1
https://fareedfauzi.gitbook.io/ctf-checklist-for-beginner/steganography


# More about steg history and methods
https://www.vskills.in/certification/tutorial/steganography-2/


# References
For tool descriptions:
https://0xrick.github.io/lists/stego/
https://www.4rth4s.xyz/2020/10/learning-audio-forensics-with-audacity.html?showComment=1646079629457
