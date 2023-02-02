
<p align="center">
<img src="https://i.imgur.com/jQBLzkg.gif" />
</p>

**SlidingTabView** is a simple Android-Like tab view that is built using the latest and greatest SwiftUI. Almost everything is customizable!

## Installation
Please use Swift Package Manager to install **SlidingTabView**

## Usage
Just instantiate and bind it to your state. That is it!
```swift
@State private var selectedTabIndex = 0
SlidingTabView(selection: $selectedTabIndex,tabs: ["First Tab", "Second Tab"]) {
    Text("First Page")
    Text("Second Page")
}
```

## Canvas Preview
```swift
struct SlidingTabConsumerView : View {
    @State private var selectedTabIndex = 0

    var body: some View {
        SlidingTabView(selection: self.$selectedTabIndex,
                       tabs: ["First", "Second"],
                       font: .body,
                       activeAccentColor: Color.blue,
                       selectionBarColor: Color.blue) {
            Text("First View")
            Text("Second View")
        }
    }
}

@available(iOS 14.0.0, *)
struct SlidingTabView_Previews : PreviewProvider {
    static var previews: some View {
        SlidingTabConsumerView()
    }
}
```
## Forked from [QuynhNguyen/SlidingTabView](https://github.com/QuynhNguyen/SlidingTabView)

This repository is a fork of [QuynhNguyen/SlidingTabView](https://github.com/QuynhNguyen/SlidingTabView), which was previously abandoned. 
I have taken over development and maintenance of this project to continue its development after attempting to reach out to the original author, but was unable to do so.

All credit for the original work goes to [QuynhNguyen](https://github.com/QuynhNguyen). I am grateful for their contributions and for making the source code available for others to use and build upon. 

## Suggestions or feedback?
Feel free to create a pull request!
