 table, th, td { border: 1px solid black; border-collapse: collapse; }

IBM Daeja ViewONE, 5.0.14 iFix 3 Readme
=======================================

This Readme document contains information about the installation of this package and about restrictions in support of IBM Daeja ViewONE, Version 5.0.14 iFix 3

Readme for: **IBM Daeja ViewONE**

Product or component release: **Version 5.0.14**

Update name: **iFix 3**

Prerequisites before installing IBM Daeja ViewONE, Version 5.0.14 iFix 3
------------------------------------------------------------------------

You must have IBM Daeja ViewONE, Version 5.0.14 installed.

Before you install IBM Daeja ViewONE, Version 5.0.14 iFix 3:

*   Install IBM Daeja ViewONE, Version 5.0.14.

*   Take a backup copy all the files in the **client** and **server** directories under the Daeja ViewONE Installation directory.

Installing IBM Daeja ViewONE, 5.0.14 iFix 3
-------------------------------------------

IBM Daeja ViewONE, 5.0.14 iFix 3 is provided as a compressed file containing the files that are needed to update Version 5.0.14 for all supported platforms.

To install this package:

1.  Unzip the compressed file into the directory where IBM Daeja ViewONE, Version 5.0.14 was installed. This action overwrites all the files that need updates in the **client/v1files** directory and the **server/WEB-INF/lib** directory.
2.  As this package contains all the files required for all platforms, you can remove the files that are included for platforms that are not relevant to your environment. Change to the **server/WEB-INF/lib** directory under the Daeja ViewONE installation directory and delete the platform specific jars that are not relevant.
    
    There are platform specific jar files:
    
    *   jiserver-resources-aix.jar - used for all supported AIX platforms
    *   jiserver-resources-linux.jar - used for all supported Linux platforms (RHEL)
    *   jiserver-resources-win32.jar - used for all supported Microsoft Windows platforms
3.  Make a backup of the Daeja ViewONE 5.0.14 files in the relevant locations in your web application server. For the server files that will be the web application's **WEB-INF/lib** directory. For the client, it will be where the package client files were copied to. For example **v1files** directory in the web application.
    
4.  Copy the client and server files into the relevant places in your web application and ensure that the application is deployed as per your web app server specific requirements.
5.  Verify that the correct version of IBM Daeja ViewONE is deployed to the web application server. This can be done by displaying the About Box in Daeja ViewONE Virtual by clicking on the **ViewONE** logo in the bottom right corner. Verify that the version number 5.0.14 iFix 3 is listed at the bottom of the About Box.

**Note:**

1.  To upgrade to iFix 3, please ensure that both the client and the server are updated.
    
2.  Ensure browser cache is deleted after IBM Daeja ViewONE is upgraded.
    

Removing IBM Daeja ViewONE, 5.0.14 iFix 3
-----------------------------------------

If you want to remove the iFix 3 from your installation and revert back to the original 5.0.14 version, you need to replace the files in you installation directories with the backed up files, then copy the files into the correct places in your web application server.

If you use the IBM Daeja ViewONE Version 5.0.14 uninstallation program to remove IBM Daeja ViewONE 5.0.14 and the iFix 3 from your system, then some of the files may be left on your file system and you will need to remove them manually.

Configuring the Viewer
----------------------

IBM Daeja ViewONE comes with a Toolkit rich in capabilities that enables advanced integration and customization of the viewer by using HTML parameters and JavaScript API methods. For more information on the developer’s guide refer to:

[IBM Daeja ViewONE 5.0.14 Virtual Developer's Guide](https://www.ibm.com/support/pages/node/295281)

Fixes in IBM Daeja ViewONE, 5.0.14 iFix 3
-----------------------------------------

The following APARs are fixed in this product release for customers who have direct entitlement to IBM Daeja ViewONE. If you are using IBM Daeja ViewONE made available to you as part of another IBM product, these fixes might not be available immediately. Contact IBM Support for information about IBM products that integrate IBM Daeja ViewONE.

Latest iFixes and readmes for this release: [https:// www.ibm.com/support/fixcentral/swg/selectFixes? parent=Enterprise%20Content%20Management&product=ibm/Other+software/ Daeja+ViewONE+Virtual&release=5.0.14&platform=All&function=all](https://www.ibm.com/support/fixcentral/swg/selectFixes?parent=Enterprise%20Content%20Management&product=ibm/Other+software/Daeja+ViewONE+Virtual&release=5.0.14&platform=All&function=all)

* * *

**DT270188 PDF Documents containing Extension B characters in form fields print incorrectly when printOriginalSize is unchecked**

When 'Extension B characters' are present in the PDF forms and printed with PrintOriginalSize option unchecked, the remaining characters following the 'Extension B characters' are not displayed in the printed document. With the fix, they are skipped and the remaining characters will be displayed in the printed document.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**DT377886 Unable to display EML files with invalid font family syntax attribute**

EML file containing unicode character 0x3 fails to open in viewer.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**DT378515 Enable font type annotations support for pageN documents**

Font selection for text annotation is not possible in PageN documents.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**DT381213 Custom stamp annotation does not show 'highlight' when it is added to the document**

While adding stamp annotation using the custom property _annotationStampProperties<N>_, the _fillcolor_ property is not working as expected.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**DT381563 Certain form fields of PDF displays text in wrong font**

Certain PDF with native annotations fails to display correct font inside form fields.

To address this, new parameter, **enablePdfNativeAnnotation** has been added to disable native annotations in PDF document by setting it to **false**

Note : Default value of this parameter is **true** which enables native PDF annotations.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**DT381877 Radio button selection is not displayed appropriately in certain PDF documents**

Some radio buttons in the PDF document are not displayed correctly in the viewer. For instance, if a PDF contains multiple groups of radio buttons on a single page, selecting a button in one group prevents selections in other groups.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**DT382050 Annotations on top of PDF form fields are not editable**

When annotations are saved on top of PDF form fields, they are not editable.

NOTE: With this fix, when PDF document contain link annotations, the links can be clicked only after enabling text selection.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

* * *

Fixes and Features released in previous iFixes and Fix Packs
------------------------------------------------------------

IBM Daeja ViewONE 5.0.14 iFix 2
-------------------------------

**DT270207 Default behavior of Custom button is not working as expected**

With the support for Content Security Policy, the functionality of custom buttons were affected due to incorrect determination of CSP enablement.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**DT364017 Unable to display EML files with invalid hypertext reference attribute**

Specific EML file with invalid hypertext reference attribute, fails to render with an error message.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**DT364993 Footer alignment and table rendering is not correct in specific MS Word documents**

Certain MS Word documents displayed incorrect alignment with respect to text and table content alongside the footer image.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29397 SETPAGE() TO THE SAME PAGE DOES NOT WORK PROPERLY WHEN CONTINUOUS PAGE VIEW IS DISABLED**

When continuousPageViewEnabled is set to false and the JavaScript function setPage() is called for the same page, the page will not be rendered .

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29423 MISSING CHARACTERS WHEN PRINTING PDF DOCUMENT WITH PRINTORIGINALSIZE OPTION UNCHECKED**

When documents are printed without the **printOriginalSize** option checked, some form fields may not appear due to missing fonts.

Font substitution can be customized by defining the **pdfFontSubstitute** HTML attribute and specifying the substitute font name.

Note: This is applicable only when parameter **PDFfontAliasesSupplied** is set to **true**

_Example : pdfFontSubstitute = 'courrier=courier,KozGoPr6N-Medium=mingliu'_

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

IBM Daeja ViewONE 5.0.14 iFix 1
-------------------------------

**IO29339 UNABLE TO OPEN A PARTICULAR MSG FILE DUE TO A PARSING ERROR**

Specific MSG file with inline expression and also different syntax for certain html attributes, fails to render with an error message.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29361 DISPLAY ISSUE WITH DOCX CONTAINING TABLES AND OTHER FORMATTING**

Certain table style, bullets and numbering, table of contents are not displayed correctly in MS Word document.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29376 SCREEN READER DOES NOT PRONOUNCE MANY BUTTON NAMES CORRECTLY**

Few buttons do not have proper aria-labels set which makes it difficult to identify using JAWS reader.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29386 ISSUE WHEN RENDERING A MS DOCUMENT (DOCX) FILE WHERE THERE IS A LOGO IN THE HEADER**

When a document has huge images such as logos in Header or Footer, entire document content was getting replaced with only the image/logo. Overlapping was very evident between the content and the image.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29403 UNABLE TO OPEN A PARTICULAR EML FILE DUE TO A PARSING ERROR**

Specific EML file with invalid row attribute, fails to render with an error message.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

IBM Daeja ViewONE 5.0.14
------------------------

**IO28920 CERTAIN PDF FILES WHEN VIEWED CAUSED BROWSER TO RUN OUT OF MEMORY**

With certain PDF Documents, with continuous scroll or navigation, the browser memory reached more than a gigabyte.

This caused the browser to crash if the system memory was less.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO28964 DOCUMENT FAILS TO OPEN WHEN DISPLAY IS NOT SET FOR CUSTOM FONT ANNOTATIONS**

When the system lacks configured DISPLAY settings, custom font annotation texts fail to function.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29322 A CERTAIN MS WORD DOCUMENT WITH CHECKBOX CONTENT IS UNRESPONSIVE DURING RENDER**

Specific word document with checkbox content, fails to render and shows the spinner for a long time eventually resulting into hung threads.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29342 JAVASCRIPT ERRORS GENERATED IN BROWSER CONSOLE WHEN USING THE GOTO PAGE FEATURE**

When goto page feature is used to navigate to different pages, javascript errors are thrown in the browser console.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29356 SPECIFIC MS WORD DOCUMENT CONTENT NOT RENDER AS NATIVE APPLICATION**

Some MS Word documents do not render the complete page content table content missing while rendering.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29360 DOCUMENT DOWNLOAD FUNCTION OF VIEWER FAILS FOR A CONTENT MANAGER REPOSITORY**

When Content Manager Enterprise Edition is the repository for documents, download function would fail in the viewer. This defect doesn't affect FileNet P8 customers.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29366 SINGLE-PAGE MS WORD FILE DISPLAYS IN MULTIPLE PAGES**

Certain single page MS word document erroneously shows as a multi page document in the viewer.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29367 CERTAIN MS WORD DOCUMENT WITH HEBREW DOES NOT RENDER AS EXPECTED**

While opening certain MS Word document containing Hebrew text, does not display content as expected.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**IO29368 ISSUE IN VIEWING PROCESSED MS WORD DOCX FILES IN VIEWER**

When certain MS Word docx files are opened in viewer, it keeps loading and the page count is observed to be incorrect.

_Affected users_: IBM Daeja ViewONE Virtual users

* * *

**CSDV-31 Display warning message for PDF documents which falls under limitation of 'Optimized performance of printing PDF documents'.**

During print process, when the application is not able to optimize the document for print, it silently switches to fallback print mechanism.

Users will now be notified with a message in the print pop-up when the application is not able to optimize the document and prints using fallback mechanism.

The message reads as:

_The document cannot be optimized for print. Printing using fallback mechanism. Preparing File_

* * *

**CSDV-51 Provide a configurable option to create temp folder for cache creation**

In this release, a new server-side parameter, tempCacheLocation, has been introduced, allowing users to specify a custom temporary cache location.

Changes to this parameter require an application server restart.

The directory location that is assigned as a value to this parameter should have appropriate read and write permissions from the server where application is running.

This is an optional confiuration. If this value is not provided, the temporary cache will continue to get created inside the app server.

Sample syntax : **_tempCacheLocation=c:/temp_**

* * *

**CSDV-60 Support for LiveCycle / Life cycle/ LifeCycle PDF Documents**

In this release, PDF documents that contain XFA forms will be displayed with restricted feature capabilities.

Please note that this is a Tech Preview of XFA Support and some functionality may not work as expected

To activate the rendering of these forms, a new HTML parameter, **_enableXFA_**, has been introduced, with default value set to false. Setting this parameter to true allows the viewing of XFA forms.

* * *

**CSDV-66 Implement footer text and positioning when printing documents**

Custom text can now be printed at the bottom of the document page and the positioning of this custom text can be specified. A new parameter **_printFooter_** can be used to specify custom text to be printed. We can also specify the alignment of the custom text with the two parameters **_printHeaderAlign_** for header text and **_printFooterAlign_** for footer text. The parameter can take the following possible values:

**left**: prints the text in the bottom left of the page.

**center**: prints the text in the bottom center of the page.

**right**: prints the text in the bottom right of the page.

The following footer options are available:

**Any Text**  
Custom text to be printed. For example, your own copyright for the documents that are being viewed or some other informational text.

**Formatted Text**  
Text can include limited formatted elements as below.

When parameter `**printFooter**` is set to **$page # $of ##**, first page will display Page 1 of 5 for a document containing 5 pages. It is to be noted that **\#** will print current page and **\##** will print the total number of pages.

* * *

**CSDV-70 Allow Daeja font file location to be configurable**

User can now configure the additional font files location which are required to select the font type in annotation toolbar.

User can generate the font files required for custom annotation font type, using a utility (daeja-font-utility.jar).

Place the utility jar and TTF files of the relevant font under the same directory (for which font files needs to be generated) and execute the jar using the command 'java -jar daeja-font-utlity.jar'.

Example: java -jar C:/Administrator/Desktop/CustomFonts/daeja-font-utlity.jar

When the font generation is complete, copy the directory path and specify it under the server parameter **annotationCustomFonts**

Example: annotationCustomFonts = C:/Administrator/Desktop/CustomFonts

Restart the web application server for the addtional fonts to be displayed in the font type dropdown within annotation toolbar.

**Download the utility [here](https://www.ibm.com/support/pages/node/7097609)**

* * *

Additional Release Notes
------------------------

### System requirements

Go to the page at [Software Product Compatibility Reports](https://www.ibm.com/software/reports/compatibility/clarity/index.html) to create a high-level report for operating systems, hypervisors and prerequisites.

### Optimized performance of printing PDF documents

When printing PDF documents with annotations, the annotations are embedded in the downloaded PDF document as native PDF annotations. This reduces the time taken to print documents, especially large documents.  
  
This process currently only applies to printing PDF documents when **'Print Original Size'** is selected in the print settings. If this is not selected or the printed document contains other file formats, the print process completely flattens the content of each page.  
  
The time it takes to prepare a PDF with annotations for print using the optimized print depends on the total number of annotations. In most cases you need to have several hundreds of annotations in a single document before the time difference becomes noticeable.  
  
With the optimized print any annotations created in IBM Daeja ViewONE Virtual are embedded into the document as native PDF annotations. Therefore they are recognized as active annotations when the PDF is viewed by tools that support editing of PDF documents. If this document is subsequently viewed by IBM Daeja ViewONE Virtual, any annotations will be treated as static content where loading a document with pre-applied native annotations cannot be edited. To prevent document or annotation modification appropriate security would need to be set via a tool that supports editing or via some PDF printers.  
  
**Sticky Notes**  
Sticky Note annotations will appear on top of other annotations regardless of z-order.  
  
**Line Width**  
The maximum line width of native annotations is 12pt and will be limited to this for print output.  
  
**Solid Text**  
If a solid text annotation is set to be semi-transparent the fill background and the text will become semi-transparent, previous behavior left the text solid and only the fill became semi-transparent.  
  
**Image Stamps**  
Image stamp annotations will appear underneath any other annotation types regardless of the z-order. This is due to the fact that they added to the content of the PDF and not as separate native PDF annotations.

#### Limitations

The optimized PDF print does not occur in the following circumstances:  

*   PDF documents with digital signatures.
*   PDF documents with password encryption and edit protection.
*   PDF Documents with any ruler or angle annotations.

### Document Builder

#### Document Builder uses repository-document and repository-annotations when the document is created

The document will be built with the source document as it is saved in the repository. The document is also built by using the annotations that are saved in the repository, unless annotations have been edited. The following scenarios explain the effects of this behavior:

##### Scenario 1:

1.  Two instances of the viewer are opened in document builder mode
2.  A document is loaded from a repository into each viewer window
3.  The document builder user copies a page from the document in viewer window 1 and pastes the page into the document in viewer window 2
4.  While the document builder user is working on the documents, another user or system process alters one or both of the master documents
5.  The document builder user builds the modified document
6.  Because one or both of the master documents were altered during the document builder session, the built document contains the pages from the latest saved version of the master documents

Result: The document currently displayed in the viewer differs from the newly built document in the system. To prevent this issue occurring, the master document should be locked or checked out when it is retrieved for document builder.

**Note** Versioned documents will not be affected by this issue. This will only affect situations where the document that a URL refers to has changed.

##### Scenario 2:

1.  Two instances of the viewer are opened in document builder mode
2.  A document with annotations is loaded from a repository into each viewer window
3.  The document builder user copies a page from the document in viewer window 1 and pastes the page into the document in viewer window 2
4.  While the document builder user is working on the document, another user or system process alters one or more of the annotations used in one or both master documents
5.  The document builder user builds the modified document
6.  The built document contains the pages from the latest saved version of the master documents. For pages where the document builder user has not modified annotations in the viewer, the annotations for those pages come from the latest saved annotations version. For pages that the user has modified the annotations in the viewer, those pages will contain annotations as seen in the viewer which may not contain the latest changes

Result: The document currently displayed in the viewer differs from the newly built document in the system. To prevent this issue occurring, the master document should be locked or checked out when it is retrieved for document builder.

#### Restore annotations is not supported in document builder mode

When in document builder mode, the option to restore annotations is not supported. The following scenario explains the effects of this behavior:

Scenario 1:

1.  Viewer is loaded in document builder mode
2.  A document is loaded from a repository
3.  Annotations are created by the user
4.  Restore annotations button is disabled
5.  Javascript API reloadAnnotations() is disabled

Result: The user cannot reload the annotations from the server. Newly created annotations and edited annotation edits remain.

To restore any newly created annotations, the user must take the following steps:

1.  Remove the page on which annotations are present that you want to restore
2.  Put the page with the original annotations on the clipboard (cut/copy)
3.  Paste the page into the new document location

### Daeja ViewONE as an Integrated solution

When running Daeja ViewONE 5.0.14 as a component inside IBM Content Navigator, the minimum supported version of ICN is 3.0.15, unless stated otherwise by the specific ICN release.

Known problems, issues, and limitations
---------------------------------------

As problems are discovered and resolved, the IBM Support team updates the Support site. By searching the Support site, you can quickly find workarounds or solutions to problems.

The following links open queries for IBM Daeja ViewONE documents on the IBM Support site:

*   [IBM Daeja ViewONE, Version 5.0.14 known problems](https://www.ibm.com/mysupport/s/topic/0TO500000002CuUGAU/daeja-viewone)
*   [All IBM Daeja ViewONE, Version 5.0.14 documents on the IBM Support site](https://www.ibm.com/docs/en/daeja-viewone/5.0.x)

Any restrictions and/or limitations of the base or fix pack release and any subsequent ifixes, still apply to this release unless stated otherwise.

### Supported File Formats in ViewONE Virtual

For information on the supported file formats refer to the tech note below. Please note that this is a live document and might get updated frequently. [https://www-01.ibm.com/support/docview.wss?uid=ibm10730429](https://www-01.ibm.com/support/docview.wss?uid=ibm10730429)

### Comparison with native renderers

IBM Daeja ViewONE Virtual is designed to support as many file types as possible. However, the product is not able to render every type of file with the same accuracy as native applications, such as Microsoft Word. The flexibility of the viewer can lead to differences in the way that the documents are displayed between the native application and the viewer. The severity of the differences varies depending on the complexity of the file type. In particular, PDF files and Microsoft Office files are difficult to render with complete accuracy in a universal viewer.

### Microsoft browser limitation

For additional information on IE/Edge limitations, refer to the following tech notes:

*   [https://www.ibm.com/support/pages/node/876592](https://www.ibm.com/support/pages/node/876592)
*   [https://www.ibm.com/support/pages/node/875492](https://www.ibm.com/support/pages/node/875492)

### Excel spreadsheet load times

Excel spreadsheet load times are impacted based on the size and complexity of the Excel document. In order to improve load times, IBM Daeja ViewONE does support tuning capabilities, such as breaking up the Excel document presentation into multiple pages. Please be aware, as this behavior may not be optimal for your end user viewing experience.

### Prompt to save redacted documents uses hexadecimal filename

After a document is permanently redacted and the user selects Download, they are normally prompted to save the document with a file name based on the original un-redacted document. For instance, `mypresentation.ppt` will default to `mypresentation.tif`. In this version the user might be prompted with a filename such as `41f96b20b97f431ebd4efd85245f1f72.tif` instead. The user can still change the name to something more meaningful.

### No pageN support in document builder mode

If a pageN document is open in the viewer, the user cannot switch to document builder mode. The user remains in the edit mode in which the document was opened. The following scenario explains the effects of this behavior:

Scenario 1:

1.  Viewer is loaded in either annotation or redaction mode
2.  A pageN document is loaded from a repository
3.  A user attempts to switch to document builder mode
4.  The user receives a message and remains in annotation or redaction mode

Result: This switch is not permitted and the user will stay in their current mode.

To enter document builder mode, the user must close the pageN document and then switch to document builder mode.

### No docN support in document builder mode

DocN documents are not supported in conjunction with document builder mode. The combination of these features may result in unusual and/or unexpected behavior.

### Document Builder supported file type limitations

Document builder is able to support TIFF and PDF files with the exception of email attachments. TIFF and PDF files that are attached to emails cannot be used as source files for a new document.

PDF files with access control flags set by the owner of the document cannot be used as a source document for document building where they require a password to view the document or where the owner has indicated that the content may not be copied.

### Rendering of the semi transparency appears to blend between the outline and the fill

Annotations that have the semi-transparent property set to true, the transparent property set to true and a fill color set can appear to blend the line and fill colors near the edges.

### Annotation with fill color set to black and set to transparent are not printed transparent

Annotations that have the transparent property set to true and a fill color set to black are not printed transparent for non PDF documents. When printing PDF documents, with 'Print Original Size' selected, these annotations are printed with transparency applied.

### UI mirroring limitation

UI mirroring is not supported for the bidi languages, Arabic and Hebrew.

Copyright and trademark information
-----------------------------------

[http://www.ibm.com/legal/copytrade.shtml](http://www.ibm.com/legal/copytrade.shtml)

Notices
-------

INTERNATIONAL BUSINESS MACHINES CORPORATION PROVIDES THIS PUBLICATION "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF NON-INFRINGEMENT, MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE. Some jurisdictions do not allow disclaimer of express or implied warranties in certain transactions, therefore, this statement may not apply to you.

This information could include technical inaccuracies or typographical errors. Changes are periodically made to the information herein; these changes will be incorporated in new editions of the publication. IBM may make improvements and/or changes in the product(s) and/or the program(s) described in this publication at any time without notice.

Other company, product, or service names may be trademarks or service marks of others.

THIRD-PARTY LICENSE TERMS AND CONDITIONS, NOTICES AND INFORMATION
-----------------------------------------------------------------

The license agreement for this product refers you to this file for details concerning terms and conditions applicable to third party software code included in this product, and for certain notices and other information IBM must provide to you under its license to certain software code. The relevant terms and conditions, notices and other information are provided or referenced below. Please note that any non-English version of the licenses below is unofficial and is provided to you for your convenience only. The English version of the licenses below, provided as part of the English version of this file, is the official version.

Notwithstanding the terms and conditions of any other agreement you may have with IBM or any of its related or affiliated entities (collectively "IBM"), the third party software code identified below are "Excluded Components" and are subject to the following terms and conditions:

*   The Excluded Components are provided on an "AS IS" basis
*   IBM DISCLAIMS ANY AND ALL EXPRESS AND IMPLIED WARRANTIES AND CONDITIONS WITH RESPECT TO THE EXCLUDED COMPONENTS, INCLUDING, BUT NOT LIMITED TO, THE WARRANTY OF NON-INFRINGEMENT OR INTERFERENCE AND THE IMPLIED WARRANTIES AND CONDITIONS OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
*   IBM will not be liable to you or indemnify you for any claims related to the Excluded Components
*   IBM will not be liable for any direct, indirect, incidental, special, exemplary, punitive or consequential damages with respect to the Excluded Components.