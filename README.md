# Foponts project
##About
Simple configuration file for Apache FOP to produce pretty pdf output using free OFL-licensed fonts.
## Usage

1. Fire up your Linux or Mac console.
2. Locate your fo-file to convert to PDF or choose the appropriate xsl/xml pair to convert directly to PDF file.
3. Converting fo-files:
```fop -c foponts.xml -fo <your_fo_file>.fo -pdf <target_pdf_file>.pdf```
4. Converting to PDF using xsl/xml pair:
```fop -c foponts.xml -xml <your_xml_file> -xsl <your_xsl_file> -pdf <target_pdf_file>.pdf```
