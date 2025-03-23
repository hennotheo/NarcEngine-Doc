---
Assembly: "[[NarcIO.dll.canvas|NarcIO.dll]]"
namespace: narc_io
dependencies:
  - "[[TinyObjLoader]]"
---
### Typedefs

- `VertexList`: A list of 3D vertices (`std::vector<glm::vec3>`).
- `ColorList`: A list of 3D colors (`std::vector<glm::vec3>`).
- `TexCoordList`: A list of 2D texture coordinates (`std::vector<glm::vec2>`).
- `IndexList`: A list of indices (`std::vector<uint32_t>`).

### Struct: [[Model3D]]
The [[Model3D]] class represents a 3D model with vertices, texture coordinates, colors, and indices.

- #DLL_EXPORT
- Final

#### Friend Classes
- [[FileReader]]

#### Attributes

- `m_vertices`: A list of 3D vertices (`std::vector<glm::vec3>`).
- `m_texCoords`: A list of 2D texture coordinates (`std::vector<glm::vec2>`).
- `m_colors`: A list of 3D colors (`std::vector<glm::vec3>`).
- `m_indices`: A list of indices (`std::vector<uint32_t>`).

#### Methods

- `uint32_t getVerticesCount() const`: Get the number of vertices in the model.
- `const VertexList* getVertices() const`: Get a pointer to the list of vertices.
- `const TexCoordList* getTexCoords() const`: Get a pointer to the list of texture coordinates.
- `const ColorList* getColors() const`: Get a pointer to the list of colors.
- `const IndexList* getIndices() const`: Get a pointer to the list of indices.
