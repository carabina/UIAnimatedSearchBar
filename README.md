# UIAnimatedSearchBar

[![CI Status](https://img.shields.io/travis/KyleBurkholder/UIAnimatedSearchBar.svg?style=flat)](https://travis-ci.org/KyleBurkholder/UIAnimatedSearchBar)
[![Version](https://img.shields.io/cocoapods/v/UIAnimatedSearchBar.svg?style=flat)](https://cocoapods.org/pods/UIAnimatedSearchBar)
[![License](https://img.shields.io/cocoapods/l/UIAnimatedSearchBar.svg?style=flat)](https://cocoapods.org/pods/UIAnimatedSearchBar)
[![Platform](https://img.shields.io/cocoapods/p/UIAnimatedSearchBar.svg?style=flat)](https://cocoapods.org/pods/UIAnimatedSearchBar)

## Description

![Alt Text](https://media.giphy.com/media/fHingtLkG7v9wZZ2YW/giphy.gif)

The UIAnimatedSearchBar is similar to the standard UISearchBar but with the added animation of the search glass. I have tried to add the same functionality that UISearchBar comes with. The cancel button and the bookmark button can both be added just like UISearchBar. Additionally there is a UIAnimatedSearchBarDelegate that mirrors the same functionality that UISearchBarDelegate offers.

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

Deployment Target: 11.0

## Installation

UIAnimatedSearchBar is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'UIAnimatedSearchBar'
```

At the end of the podfile add this post_install to allow the @IBDesignable aspect of the UIAnimatedSearchBar to work:

```ruby
# Workaround for Cocoapods v.1.5 issue #7606
post_install do |installer|
    installer.pods_project.build_configurations.each do |config|
        config.build_settings.delete('CODE_SIGNING_ALLOWED')
        config.build_settings.delete('CODE_SIGNING_REQUIRED')
    end
end
```

UIAnimatedSearchBar can be added with either Interface Builder or it can be done programatically.

## Author

Kyle Burkholder  
Email: kburkho@gmail.com  
Twitter: [_KyleBurkholder](https://twitter.com/_KyleBurkholder)  
Follow me on Twitter. I'd love to see what other ios developers are working on.

## Donations

I'm a self taught ios programmer and if you want to see more things like this feel free to buy me a cup of coffee, or two. ;)

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GACPM42EKYZDU)

## License

UIAnimatedSearchBar is available under the MIT license. See the LICENSE file for more info.

