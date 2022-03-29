# foponts FAQ

## Why foponts and what does it mean?

Because it's quite simple and sounds good :)

The name of the project is originated and formed from the name of the Apache project ("FOP") and a word "fonts".

## Why foponts was created?

Short answer: to make things easy.

Long answer:
The author of the _foponts_ project is a technical writer/documentation engineer by profession. He primary uses [DocBook/XML](https://docbook.org/) as a source for documentation (of course, he sometimes also uses lightweight markup languages like asciidoc, ReStructured text, Markdown).

To get a `.pdf` files from DocBook sources the most affordable (actually, free) software is [FOP](https://xmlgraphics.apache.org/fop/) from Apache Software Foundation.

The problem was, that an earlier versions of FOP (v.0.93 - v.1.0, within a period of 2007-2009) needed to be configured hardly to work with the characters beyond the ordinary Latin alphabet (author widely uses documents with a Cyrillic alphabet).

Moreover, after implementing fonts autodetect feature (`<auto-detect/>`) in a later versions of FOP, rendering results became totally unpredictable. That is because autodetection feature discovers fonts to use within *local* machine but fonts sets can differ from machine to machine. That led to a situation when one document with the same text and structure looked different while rendering on a machine X and on a server Y.

To take a rendering process under full control author decided to create a configuration file that gives totally predictable result for rendering documents irrespective the machine and/or server used for a rendering process.

As a result:

- rendered PDF documents uses only fonts that are available, well known, pre-checked for visual impression and character sets (Cyrillic, Greek, etc);

- patent- or license-related issues (if any) with a rendered documents are eliminated due to an [OFL licensed](https://scripts.sil.org/cms/scripts/render_download.php?format=file&media_id=OFL_plaintext&filename=OFL.txt) fonts are used everytime and everywhere.

## I'm scared about downloaded fonts from the author's website. It can be a fraud!

If you are really scare about it, here is a list with direct links to homepages of fonts used in a foponts project. You can download it separately and use it without any scare :)

**NOTE**: This case assumes that you take your time and put some efforts into grabbing all fonts in one place and configuring _foponts_ completely manually. Sometimes it requires compiling fonts from theirs sources! How to do this is completely out of scope of the current or any other document within a _foponts_ project.

1. **Galatia SIL**: [font homepage](https://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=GalatiaSIL).
2. **Charis SIL**: [font homepage](https://software.sil.org/charis/).
3. **Liberation** [source files](https://github.com/pravins/liberation-fonts). **NOTE**: you have to compile them from source using [FontForge](https://fontforge.github.io/en-US/).
4. **Free monospaced** [font download page](http://ftp.gnu.org/gnu/freefont/).

## How can I contact the author?

Just drop me a line to eduard.tibet@gmail.com with a "foponts" in subject line. I'm very curious to hear about your usage of **foponts**.