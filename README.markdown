NSString+JCURLUtilities

This category adds an additional instance method -queryStringDictionary to
NSString.

    // Example:
    NSURL *url = [NSURL URLWithString:@"http://intridea.com/?foo=bar#baz=garply"];
    [[url fragment] queryStringDictionary];  # { 'foo' = 'bar'; }
    [[url query] queryStringDictionary];  # { 'baz' = 'garply'; }
