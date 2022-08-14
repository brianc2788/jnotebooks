<!DOCTYPE markdown>
<!--
Steghide "How-To" Guide, written with Markdown.
---
Authored by brianc2788@gmail.com
http://brianc2788.github.io
-->
#### HOW TO USE STEGHIDE ####
Steghide is a stegonography program that hides
your messages in a few image formats and an
audio format. It uses a few sub-commands.

---
## Embed ##
***$ steghide embed -cf <cover-file> -ef <embed-file>***
**cover file** AU,BMP,JPEG images, WAV audio clips.
**embed file** file containing stuff to embed; i.e. plaintext/ASCII file.
**-e option** specift encryption algo, encinfo command.

---
## Extract ##
***$ steghide extract -sf <stegfile>***
**stegfile** A.k.a., a file with data encrypted & embedded into it w/steghide.

---
## Getting Info ##
***$ steghide info <stegfile>***

*Example output:*
"mos-tech.jpg":
  format: jpeg
  capacity: 10.1 KB
  embedded file "msg1.txt":
    size: 17.0 Byte
    encrypted: rijndael-128, cbc
    compressed: yes
