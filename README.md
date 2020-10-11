# dart_structured_data
A collection of functions for parsing structured data from web pages

# Usage
The library supports microdata, rdfa, and jsonld.
To parse structured data from a web page:
    List<StructuredData> data = await StructuredDataImporter.importUrl("path/to/website");

To parse structured data from an already loaded web page
    List<StructuredData> data = StructuredDataParser.extract(htmlDocument);

`StructuredData` is a dictionary-like object
    StructuredData someData;
    // Load data by importing from URL
    someData["property"]

# Future Improvements
Eventually I may overlay some wrapper classes for accessing structured data so it's more than
a glorified map.