# MvcRazorToPdf

Create PDF documents within an ASP .Net MVC project by generating your views as normal but returning a `PdfActionResult`.

This converts regular produced razor/html to PDF documents in the browser using the iTextXmlWorker.

This uses the newer version/licence of iText/iTextXmlWorker and can process the html that is produced from your views.

## Installation instructions:

Run the following nuget command from your mvc project to install the [package][nuget]:

`Install-Package MvcRazorToPdf`

[nuget]: http://nuget.org/packages/MvcRazorToPdf/

## How to use it

1. Create a shared layout that is compatible with an `iTextXmlWorker` document [Simple example layout][example1]
2. Create a controller action that return a `PdfActionResult` (model optional) [Simple example contoller][example2]
3. Create the view page to render as normal [Simple example view][example3]

[Complete example project](https://github.com/andyhutch77/MvcRazorToPdf/tree/master/MvcRazorToPdfExample)

[example1]: ./MvcRazorToPdfExample/Views/Shared/_PdfLayout.cshtml
[example2]: ./MvcRazorToPdfExample/Controllers/PdfController.cs
[example3]: ./MvcRazorToPdfExample/Views/Pdf/Index.cshtml

## Dependencies

	<dependency id="iTextSharp" version="5.5.5" />
	<dependency id="itextsharp.xmlworker" version="5.5.5" />

## Useful info

 * [iTextXmlWorker docs](http://demo.itextsupport.com/xmlworker/itextdoc/flatsite.html).
 * <http://demo.itextsupport.com/xmlworker/> if you have problems getting certain styles to render.
