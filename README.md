# Jamun-Scanner

Scanner is a collection of Beautiful Activity which help others to make there own Custom QR/Barcode Scanner.

### Introduction

* 

### What's New? (0.0.1)
* Stable **Official Version** for Developers and Live Apps.
* Tags to Customize Library for Any kind like **Only Barcode** or **Only QR** or **All-in-One**
* Easy Calling Mechanism with **Instant reply** via onActivityResult.
* Need less calls with many customs Tags in Intent Object to reach maximum developer satisfaction.

### Why this library?

* This library Competible with all screen sizes and device (Tab with 7' inches and 10'inches).
* Library support both orientation that is portrait and landscape.
* Its Calling feature is very simple and easy to use.
* You don't need to add Multiple libraries and UI components, it have such Components inside that make Quality.
* Library is Customizable for **Only Barcode** or **Only QR** or Any QR/Barcode Related Types.

### Quality Measures? for (0.0.1)

The following apps are using this library without facing any kind of Bugs.

* **[QR/BarcodeScanner](https://play.google.com/store/apps/details?id=ai.scanners)**
* **[ZINI](https://play.google.com/store/apps/details?id=ai.zini)**

------

### Jamun-Scanner Preview

Window View | Working Preview
---- | ----
![jamun_scanner](https://user-images.githubusercontent.com/38988514/40280595-9889b85c-5c73-11e8-9c76-3dc3a4736de6.png) | ![scanner](https://user-images.githubusercontent.com/38988514/40280291-6337c32e-5c6e-11e8-9d44-a04a519b4c96.gif)

### Gradle Configuration

**Add the dependency**

```java
dependencies {
     compile 'tk.jamun:scanner:0.0.1'
}
```
### Maven Config

```xml
<dependency>
  <groupId>tk.jamun</groupId>
  <artifactId>scanner</artifactId>
  <version>0.0.1</version>
  <type>aar</type>
</dependency>
```
------

### How to Implement

Once the project has been added to gradle, You can use these lines of code to configure pickers....

#### Step 1. Define Intent Object

Simple Object declaration :

```
Intent intent = new Intent(ActivityScannerSample.this, ActivityQrReader.class);

```
#### Step 2. Start Module By Calling

This method is very common to Android Developer, Very easy calling way to Start an activity help you same for calling this Picker :

```
startActivityForResult(intent, ACTION_QR_READER);

```

#### Step 3. Get Result from Picker

```
@Override
public void onActivityResult(int requestCode, int resultCode, Intent data) {
super.onActivityResult(requestCode, resultCode, data);
 if (requestCode == ACTION_QR_READER) {
     if (resultCode == RESULT_OK) {
        String qrCode = data.getStringExtra(INTENT_FOR_CODE);
     }
  }
}
```

### Picker Customize 

Intent Object provide you custom functionality to work Module according to your requirement :

#### Set Title of the Date Picker

By Defining this tag with String can help you setting Title of the date Picker.

```
intent.putExtra(INTENT_SCANNER_ACTIVITY_NAME, "Title of the Scanner Activity");
```

#### Set Type of Scanner

By Defining this tag you can set Your Scanner Behave, There are two of its Kind :-

* **SCANNER_TYPE_BARCODE** : for Bracode
* **SCANNER_TYPE_QR** : for QR

```
intent.putExtra(INTENT_SCANNER_TYPE, SCANNER_TYPE_BARCODE);
```

#### Set Type of Scanner

By Defining this tag you can set Your Scanner Behave, There are two of its Kind :-

For All Format : --
* **TYPE_ALL_FORMAT

For BARCODE Format : --
* **YPE_BARCODE_CODE_128
* **TYPE_BARCODE_CODE_39
* **TYPE_BARCODE_CODE_93
* **TYPE_BARCODE_CODABAR
* **TYPE_BARCODE_EAN_13
* **TYPE_BARCODE_EAN_8
* **TYPE_BARCODE_ITF
* **TYPE_BARCODE_UPC_A
* **TYPE_BARCODE_UPC_E

For QR Format : --
* **TYPE_QR_CODE
* **TYPE_QR_PDF417
* **TYPE_QR_DATA_MATRIX
* **TYPE_QR_AZTEC

```
intent.putExtra(INTENT_SCANNER_TYPE, TYPE_ALL_FORMAT);
```

------

# Dependency

* Goole Vision ``v15.0.2``
* Zxing ``3.3.0``
* SDK Version ``15 to 27``

## Credits

Desgin & Developed by : **[Jatin Sahgal](https://www.linkedin.com/in/jatinsahgal/)**
 (**[Linkedin](https://www.linkedin.com/in/jatinsahgal/)** & **[Website](https://jatin.techcruzers.com)**) 

Content Writer : **[Achal Garg](https://www.linkedin.com/in/techgarg/)**
 (**[Linkedin](https://www.linkedin.com/in/techachal/)** & **[Website](https://achal.techcruzers.com)**) 

Company : **[Techcruzers](https://www.techcruzers.com)**

## More Library under Jamun 

* **[Pickers](https://github.com/Lib-Jamun/Pickers.git)**
Pickers Library provide you a set of Pickers like Country, Language, Share and Intent Chooser.

* **[Country-Pickers](https://github.com/Lib-Jamun/Pickers.git)**
allow you to access Country picking functionality with great UI/UX design, and there are numberous of function which help you to modify picker as per your requirements. Library has been provided with four custom UI initate mode you can decide how the view of picker can be initate. You can also decide weather picker inheriate Single or Multi Selection property. Library consists of updated collection of country name, code and there flags. We are using APIs base structure to avoid increase in the size of apk due to flag Images. This module Maintain the database so that you don't need to call APIs again and again rather than you can choose when to refresh the Database and fetch new real time data.

* **[Language-Pickers](https://github.com/Lib-Jamun/Pickers.git)**
provides you read-made Language picker  which is easy to use and comes with great UI/UX, and there are numberous of function which help you to modify picker as per your requirements. Library has been provided with four custom UI initate mode you can decide how the view of picker can be initate. You can also decide weather picker inheriate Single or Multi Selection property.

* **[Calendar](https://github.com/Lib-Jamun/calendar.git)**
is a collection of Beautiful Activities which help others to make there Fully Custom Calendar View with Single and Multi Date Picker Functionality.

* **[Scanner](https://github.com/Lib-Jamun/scanner.git)**
is a collection of Beautiful Activity which help others to make there own Custom QR/Barcode Scanner. 

* **[Volley](https://github.com/Lib-Jamun/Volley.git)**
Library is a set of Custom Classes with UI components for network programming, integration and transaction handling in a better and standard way. This will help developers for making quality use of volley library. 

* **[UI](https://github.com/Lib-Jamun/ui.git)**
library is a set of UI Views, Custom Component and Collection of Helper Classes which help Developer for making quality Product. Such as Camera, Gallery, Number of Pickers, Calendar, Date Pickers, Dialogs and many more Heler UI and Backend Component.

* **[Camera](https://github.com/Lib-Jamun/ui.git)**
library provide you Custom Complete Camera view with full features like Flash, Rotation, Gallery Picker, Focus, Tap to capture, Confirmation window and last but not least croping feature. It also provide you file path in return so that developer can feel a friendly handy way to Deal After. 

* **[Gallery](https://github.com/Lib-Jamun/ui.git)**
have some Beautiful UI Components and Multi files Mode for android Developers to give there app a A Rich look With single and Multi picker Functionality.


## License
    Copyright (c) 2018 Jatin Sahgal

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
  
  
