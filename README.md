# Splunk Extension for Visual Studio
## Version 1.0

The Splunk Extension for Visual Studio adds project templates to Visual Studio
to help in writing programs that access Splunk via the Splunk SDK for C# and
writing modular inputs for Splunk in C#.

Splunk is a search engine and analytic environment that uses a distributed
map-reduce architecture to efficiently index, search, and process large 
time-varying data sets.

The Splunk product is popular with system administrators for aggregation and
monitoring of IT machine data, security, compliance and a wide variety of 
other scenarios that share a requirement to efficiently index, search, analyze,
and generate real-time notifications from large volumes of time series data.

The Splunk developer platform enables developers to take advantage of the 
same technology used by the Splunk product to build exciting new applications
that are enabled by Splunk's unique capabilities.

## Supported platforms

The Splunk Extension for Visual Studio requires Visual Studio 2012 or 2013.

## Getting started with the Splunk extension for Visual Studio

You can install the Splunk Extension for Visual Studio from the Visual
Studio Gallery. You will also need an installation of
Splunk Enterprise to test the code you write using the extension.

### Installing from the Visual Studio Gallery

1. In Visual Studio, on the Tools menu, click Extensions and Updates.

2. In the Extensions and Updates dialog box, in the left pane, expand 
   Online and click Visual Studio Gallery.

4. In the Search Visual Studio Gallery box in the right pane, type splunk. 
   "Splunk extension for Visual Studio" appears in the middle pane.

5. Click the Download button next to the extension's name.

6. In the Download and Install dialog box, click Install.

7. Click the Restart Now button that appears at the bottom of the Extensions and Updates dialog box to restart Visual Studio.

### Getting Splunk Enterprise

If you haven't already installed Splunk Enterprise, download it at 
<http://www.splunk.com/download>. For more information about installing and 
running Splunk Enterprise and system requirements, see the
[Splunk Installation Manual](http://docs.splunk.com/Documentation/Splunk/latest/Installation). 

#### Getting the source

[Get the Splunk extension for Visual Studio](https://github.com/splunk/splunk-extension-visualstudio/archive/master.zip). Download the ZIP file and extract its contents.

If you are interested in contributing to the Splunk extension for Visual Studio, you can 
[get it from GitHub](https://github.com/splunk/splunk-extension-visualstudio) and clone the 
resources to your computer.

#### Building the extension

To build from source after extracting or cloning the extension, do the following

1. Download and install the Visual Studio SDK.
     For Visual Studio 2012: http://www.microsoft.com/en-us/download/details.aspx?id=30668
	 For Visual Studio 2013: http://www.microsoft.com/en-us/download/details.aspx?id=40758
2. At the root level of the **splunk-extension-visualstudio** directory, open
   the **SplunkExtensionVisualStudio.sln** file in Visual Studio.
3. On the **BUILD** menu, click **Build Solution**.

This will build the extension.

#### Solution Layout

The solution is organized into five projects:

* **SplunkExtensionVisualStudio** represents the VSIX file to build, and contains all
  the NuGet packages to be included in that VSIX.
* **SplunkCSharpProjectTemplate** defines the project template for Splunk SDK for C# PCL projects.
* **CSharpProjectWizard** defines the project creation wizard for the Splunk SDK for C# template.
* **SplunkModularInputProjectTemplate** defines the project template for creating
  modular inputs.
* **ModularInputWizard** defines the project creation wizard for the modular input template.

### Changelog

The **CHANGELOG.md** file in the root of the repository contains a description
of changes for each version of the extension. You can also find it online at
[https://github.com/splunk/splunk-extension-visualstudio/blob/master/CHANGELOG.md](https://github.com/splunk/splunk-extension-visualstudio/blob/master/CHANGELOG.md). 

### Branches

The **master** branch always represents a stable and released version of the extension.
All development is merged to the **develop** branch between releases.

## Documentation and resources

If you need to know more:

* For all things developer with Splunk, your main resource is the [Splunk
  Developer Portal](http://dev.splunk.com).

* For more about the Splunk REST API, see the [REST API 
  Reference](http://docs.splunk.com/Documentation/Splunk/latest/RESTAPI).

* For more about about Splunk in general, see [Splunk>Docs](http://docs.splunk.com/Documentation/Splunk).

## Community

Stay connected with other developers building on Splunk.

<table>

<tr>
<td><em>Email</em></td>
<td><a href="mailto:devinfo@splunk.com">devinfo@splunk.com</a></td>
</tr>

<tr>
<td><em>Issues</em>
<td><a href="https://github.com/splunk/splunk-extension-visualstudio/issues/">
https://github.com/splunk/splunk-extension-visualstudio/issues</a></td>
</tr>

<tr>
<td><em>Answers</em>
<td><a href="http://splunk-base.splunk.com/tags/csharp/">
http://splunk-base.splunk.com/tags/csharp/</a></td>
</tr>

<tr>
<td><em>Blog</em>
<td><a href="http://blogs.splunk.com/dev/">http://blogs.splunk.com/dev/</a></td>
</tr>

<tr>
<td><em>Twitter</em>
<td><a href="http://twitter.com/splunkdev">@splunkdev</a></td>
</tr>

</table>

### Contributions

If you want to make a code contribution, go to the 
[Open Source](http://dev.splunk.com/view/opensource/SP-CAAAEDM)
page for more information.

### Support

1. You will be granted support if you or your company are already covered 
   under an existing maintenance/support agreement. Send an email to 
   _support@splunk.com_ and include "Splunk extension for Visual Studio" in the subject line. 

2. If you are not covered under an existing maintenance/support agreement, you 
   can find help through the broader community at:

   <ul>
   <li><a href='http://splunk-base.splunk.com/answers/'>Splunk Answers</a> (use
    the <b>visualstudio</b> tag to identify your questions)</li>
   <li><a href='http://groups.google.com/group/splunkdev'>Splunkdev Google 
    Group</a></li>
   </ul>
3. Splunk will NOT provide support for the extension if its code has been modified.
   If you modify the extension and want support, you can find help through the broader 
   community and Splunk answers (see above). We would also like to know why you modified 
   the code&mdash;please send feedback to _devinfo@splunk.com_.
4. File any issues on [GitHub](https://github.com/splunk/splunk-extension-visualstudio/issues).

### Contact Us

You can reach the Dev Platform team at devinfo@splunk.com.

## License

The Splunk extension for Visual Studio licensed under the Apache License 2.0. Details can be 
found in the LICENSE file.
