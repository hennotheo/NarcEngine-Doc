---
Assembly: "[[NarcIO.dll.canvas|NarcIO.dll]]"
namespace: narc_io
dependencies:
  - "[[STBLIB]]"
---
### Struct: [[Image]]

The [[Image]] class represents an image with width, height, channels, and pixel data.
- #DLL_EXPORT
- Final

#### Destructor

```C++
~Image()
```

Releases the image data using [[FileReader]]::releaseImage.

#### Methods

- `int getWidth() const`: Get the width of the image.
- `int getHeight() const`: Get the height of the image.
- `int getChannels() const`: Get the number of channels in the image.
- `void* getData() const`: Get a pointer to the image data.

#### Private Constructor

```C++
Image(int width, int height, int channels, void* data)
```

Constructs an [[Image]] with the specified width, height, channels, and data.

#### Attributes

- `int m_width`: The width of the image.
- `int m_height`: The height of the image.
- `int m_channels`: The number of channels in the image.
- `void* m_data`: A pointer to the image data.
