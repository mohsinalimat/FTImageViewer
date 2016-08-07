# FTImageViewer


[![Twitter](https://img.shields.io/badge/twitter-@liufengting-blue.svg?style=flat)](http://twitter.com/liufengting) 
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/liufengting/FTImageViewer/master/LICENSE)
[![Pods Versions](https://img.shields.io/cocoapods/v/FTImageViewer.svg?style=flat)](http://cocoapods.org/pods/FTImageViewer)
[![CI Status](http://img.shields.io/travis/liufengting/FTImageViewer.svg?style=flat)](https://travis-ci.org/liufengting/FTImageViewer)
[![Swift Version Compatibility](https://img.shields.io/badge/swift2-compatible-4BC51D.svg?style=flat-square)](https://developer.apple.com/swift)
[![swiftyness](https://img.shields.io/badge/pure-swift-ff3f26.svg?style=flat)](https://swift.org/)
[![Swift Version](https://img.shields.io/badge/Swift-2.2-orange.svg?style=flat)](https://swift.org)
[![GitHub stars](https://img.shields.io/github/stars/liufengting/FTImageViewer.svg)](https://github.com/liufengting/FTImageViewer/stargazers)


`FTImageViewer` can preview images with just one lines of code. Also `FTImageViewGrid` is made for images to show in grid much easier. I wrote this for my future projects. Feel free to try it in your own projects!

# Feathers

* [x] Double tap to zoom in and double tap again to zoom out
* [x] Pinch to zoom in/out
* [x] Button tap to dismiss
* [x] Button tap to save current image to system Photo Album
* [x] Pan up/down to dismiss (like Facebook or QQZone)
* [ ] Pan left/right to dismiss at first/last page

## ScreenShots

<table>
  <tr>
    <th><img src="/ScreenShots/Demo1.gif" width="250"/></th>
    <th><img src="/ScreenShots/Demo2.gif" width="250"/></th>
    <th><img src="/ScreenShots/Demo3.gif" width="250"/></th>
  </tr>
</table>

run the demo in `FTImageViewerDemo` to see more

##Usage

* show images in  a grid and preview images with one line of code 

```swift
        imageGridView.showWithImageArray(imageArray) { (buttonsArray, buttonIndex) in
            // in this tap block, preview images with one line of code
            FTImageViewer.sharedInstance.showImages(self.imageArray, atIndex: buttonIndex, fromSenderArray: buttonsArray)
        }
```
* see more docs in `FTImageViewerDemo/DemoTableViewCell.swift` 

##Installation

###Manually

* clone this repo.
* Simply drop the `FTImageViewer` folder into your project.
* Enjoy！ 

###Cocoapods

`FTImageViewer` is available through [CocoaPods](http://cocoapods.org). To install it, simply add the following line to your Podfile:

```ruby
pod 'FTImageViewer'
```

# Bonus

In `FTImageViewerDemo`, shows you how to use it in tableview, using pure `AutoLayout`. Here is the screenshot:

<table>
  <tr>
    <th><img src="/ScreenShots/autolayout1.PNG" width="250"/></th>
    <th><img src="/ScreenShots/autolayout2.PNG" width="250"/></th>
    <th><img src="/ScreenShots/autolayout3.PNG" width="250"/></th>
  </tr>
</table>

## License

`FTImageViewer` is available under the MIT license. See the `LICENSE` file for more info.

