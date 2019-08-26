About:

Placeholder Dropdown turns placeholder name input boxes into autocomplete/typeahead dropdown select lists making it easy to remember if your placeholder was called three-col-left or three-column-left and avoid typos.

Features:

Placeholder Dropdown 3.0.0 creates a placeholder autocomplete/typeahead dropdown on the select rendering dialog as well as the control properties dialog.

Installation:

Placeholder Dropdown is installed via a Sitecore package zip file.

Requirements:

Sitecore 8.0 or greater
- Version 3.0.0A works for v8.0 - v8.1
- Version 3.0.0B works for v8.2+
Sitecore itemapi access

Configuration:

1. Add your placeholders to the content tree under /sitecore/Layout/Placeholder Settings.

2. In your Sitecore config file, ensure that your main website has the following properties:

itemwebapi.mode="Off" 
itemwebapi.access="ReadOnly" 
itemwebapi.allowanonymousaccess="false"

These settings hide the itemapi from anonymous visitors, but not from authenticated users.  Your site may require additional access to the itemapi that are compatible with Placeholder Dropdown 3.0.0.

Troubleshooting:

If you are not seeing the placeholder dropdown, check the console logs and ensure that you are able to access the itemapi.

Uninstallation:

1. Remove //Website/sitecore/shell/Override/Applications/Content Manager
2. Remove //Website/sitecore/shell/Override/Applications/Dialogs/SelectRendering
3. Remove //Website/sitecore/shell/Override/Controls/AutocompleteJS
4. Remove //Website/sitecore/shell/Override/Controls/PlaceholderDropdownJS
5. Update item core::/sitecore/layout/Layouts/Applications/Field Editor ({436C5B71-21E8-4A79-96D0-FC21DC8D2B77}) and set the Path field to "/sitecore/shell/applications/Content Manager/FieldEditor.aspx"

Contact:

Twitter: @eric_sanner
Email: eric [dot] sanner [at] perficient [dot] com

Thanks:

Special thanks to Brandon Bruno for helping me to build and test this module.

License:

MIT License. 

Copyright 2018 - 2019 Eric Sanner

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
