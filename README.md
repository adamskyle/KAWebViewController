# KAWebViewController
 
KAWebViewController is a view controller class for UIWebView. Currently, KAWebViewController only works in a UINavigationController.
I never found a similar solution that suited my needs so I decided to write my own basic UIWebViewController Class.

Feel free to use this as base for your own UIWebView ViewController.
This class currently supports:

- iPad and iPhone
- iOS 6.1 to 7.1 (iOS6 on iPad could use some UI improvements)
- Portrait & Landscape mode

## Installation
 
Simply drag the KAWebViewController folder to your project. If this project evolves, I will gladly support CocoaPods installation.
 
## Usage

Use of the Storyboard Segues is recommended. So don't forget to set KAWebViewController as the custom class of your destination ViewController.

###Step 1
Import the header file in the class you want to use KAWebViewController
'#import KAWWebViewController'

###Step 2
Currently there are two ways to fire off your KAWebViewController. Via a designated initializer:
`[[KAWebViewController alloc] initWithURL:yourNSURL];`

Or via the setter (cleaner when used in prepareForSegue:):
```objc
KAWebViewController *kaw = (KAWebViewController *)segue.destinationViewController;
kaw.url = yourURL;
```

Pushing the ViewController programmatically works, but it is not supported.

## Roadmap

I do not know how far I want this project to go. 

- Support Modal Segue (definitely!)
- Automatically mimic the application UI. (Optional, via property?)
- Improved activity center
- Suggestions?
 
## Contributing
 
If you think this is a solid base for something more awesome, feel free to contribute to this project.
Fork and tinker to your own needs or submit a pull request. Keep in mind that I want to keep this project as clean, update-proof and lightweight as possible. Simplicity is the key.

You can always contact me via e-mail: kpe.adams@gmail.com
 
## History
 
- 11/4/2014: Initial release (0.1)
 
## Credits
 
Currently KAWebViewController is brought to you by Kyle Adams.
 
## License (MIT)

Copyright (c) 2014 Kyle Adams

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.