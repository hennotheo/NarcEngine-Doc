---
Assembly: "[[NarcIO.dll.canvas|NarcIO.dll]]"
namespace: narc_io
dependencies:
---
### Class: [[FileReader]]

The `FileReader` class provides static functions for reading files, loading 3D models, and reading images. It also includes a function to release image data.
- #DLL_EXPORT
- Final

#### Static Destructor

```C++
~FileReader() = delete;
```
The default constructor is deleted.

#### Static Methods

- static std::vector<char> readFile(const std::string& filename): Reads the contents of a file and returns it as a vector of characters. 
- static [[Model3D]] load3DModel(const std::string& filename): Loads a 3D model from a file.
- static [[Image]] readImage(const std::string& filename): Reads an image from a file.
- static void releaseImage(void* imageData): Releases the memory allocated for image data.