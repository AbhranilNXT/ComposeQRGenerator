# QR Generator Compose Library

A Jetpack Compose Library which can be used to generate QR Codes from texts.

## Badges

[![](https://jitpack.io/v/AbhranilNXT/ComposeQRGenerator.svg)](https://jitpack.io/#AbhranilNXT/ComposeQRGenerator)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)

## 🚀 About the Library

This Library can be used to generate QR Codes in any Android Applications from a text or url. It can be used by calling the function `qrGenerator(content = "<your_text>"` inside the painter parameter of the
Image composable as `Image(painter = qrGenerator(content = "<your_text>"), contentDescription = "QR Image")`. Additional parameters of the qrGenerator function include size and padding which can be used as 
`qrGenerator(content = "<your_text>", size = <your_size>.dp, padding = <your_padding>.dp)`

## Implementation

Add it to your `settings.gradle.kts` file using:
```gradle
dependencyResolutionManagement {
    repositories {
        maven { url = uri("https://jitpack.io") }
    }
}
```
and in your `build.gradle.kts` file using:

```gradle
dependencies {
    implementation("com.github.AbhranilNXT:ComposeQRGenerator:1.1.0")
}
```
## Demo Usage

Refer to the below code for using this library :

```kotlin
@Composable
fun Demo() {
    Surface(modifier = Modifier.fillMaxSize()) {
        Image(painter = qrGenerator(content = "https://github.com/AbhranilNXT/ComposeQRGenerator",
            size = 300.dp,
            padding = 8.dp), contentDescription = "Demo QR")

    }
}
```

The above code upon execution gets displayed as : 

![App Screenshot](https://i.postimg.cc/RZR84NKc/Screenshot-2024-03-12-025400.png)

## Author

- [Abhranil Dasgupta](https://github.com/AbhranilNXT)

## License

[GPL 3.0](https://github.com/AbhranilNXT/Scavenger-Hunt-Clone?tab=GPL-3.0-1-ov-file#readme)


## Feedback

If you have any feedback, please reach out to us at abhranilnxt@gmail.com


## Platforms/softwares(s) used to develop this:

**Android:** Android Studio, Jetpack Compose, ZWing, BitMap Painter



## Source Code

To clone this repo and look into the source code, go to the terminal in your workspace and then type

> https://github.com/AbhranilNXT/ComposeQRGenerator




## Contributing

Contributions are always welcome!

Please adhere to this project's `code of conduct`.
