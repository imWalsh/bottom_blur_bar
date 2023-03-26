<a href="https://developer.android.com" style="pointer-events: stroke;" target="_blank">
<img src="https://img.shields.io/badge/platform-Android-deepskyblue">
</a> 
<a href="https://developer.apple.com/ios/" style="pointer-events: stroke;" target="_blank">
<img src="https://img.shields.io/badge/platform-iOS-deepskyblue">
</a>
<a href=""><img src="https://app.codacy.com/project/badge/Grade/dc683c9cc61b499fa7cdbf54e4d9ff35"/></a>
<a href="https://github.com/imWalsh/bottom_blur_bar/LICENSE" style="pointer-events: stroke;" target="_blank">
<img src="https://img.shields.io/github/license/imWalsh/bottom_blur_bar">
</a>


# Preview

![bottom_blur_bar](https://github.com/imWalsh/bottom_blur_bar/bottom_blur_bar.gif)


## Basic Usage

Import it to your project file

```
import 'package:bottom_blur_bar/bottom_blur_bar.dart';
```

And add it in its most basic form like it:

```
bottomNavigationBar: BlurNavbar(
  onTap: (idx) => setState(() {
    _idx = idx;
    debugPrint('$idx');
  }),
  items: [
    BlurNavbarItem(icon: Icon(Icons.home, color: color, size: 24), title: "SEARCH"),
    BlurNavbarItem(icon: Icon(Icons.search, color: color, size: 24), title: "SEARCH"),
    BlurNavbarItem(icon: Icon(Icons.notifications, color: color, size: 24), title: "NOTIFICATIONS"),
    BlurNavbarItem(icon: Icon(Icons.local_library_rounded, color: color, size: 24), title: "LIBRARY")
  ],
  currentIndex: _idx,
  selectedColor: Colors.cyanAccent,
)
```

### Required parameters of BlurNavbar
------------

| Parameter  |  Description  |
| ------------ |  ------------ |
| onTap | Tap Event |
| items | The collection of sub-controls to be displayed |

### Optional parameters of BlurNavbar
------------

| Parameter |  Default | Description  |
| ------------ | ------------ | ------------ |
| style | auto | Blur Effect Style |
| selectedColor | -- | Defines the color of the selected |
| borderRadius | 24 | Defines the corner radius of the border |
| currentIndex | 0 | Defines the index of the selected |
| fontSize | 10 | Defines the size of the font |
| iconSize | 40 | Defines the size of the icon |

LICENSE!
------------
**bottom_blur_bar**
is [MIT-licensed.](https://github.com/imWalsh/bottom_blur_bar/LICENSE)

