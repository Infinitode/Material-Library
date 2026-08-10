# Material Library

[![Official Website](https://img.shields.io/badge/Website-infinitode.netlify.app-blue)](https://infinitode.netlify.app/resources/material-library)
[![Blender Version](https://img.shields.io/badge/Blender-3.3%2B%20%7C%203.4%2B-orange)](https://www.blender.org/)

A free resources project containing procedurally generated Blender materials for metals, deformed metals, glass, experimental textures, and more. All materials were automatically generated using a custom-coded Blender add-on.

Check out the full library and interactive showcase on our [Official Website](https://infinitode.netlify.app/resources/material-library).

## Features & Compatibility

- **100% Procedural**: All materials are built with Blender node trees without external image textures.
- **Blender Compatibility**: Compatible with **Blender 3.3 LTS, 3.4, and all newer versions**.
- **Categories Included**:
  - **Metals**: Clean, brushed, and metallic surfaces.
  - **Deformed Metals**: Dent, rusted, hammered, and warped metallic finishes.
  - **Glass**: Refractive, frosted, tinted, and textured glass shaders.
  - **Experimental & Others**: Unique pattern experiments and procedural abstracts.

## Repository Structure

```
├── blend-files/      # Contains          downloadable .blend files for each material
├── materials/        # Preview images in WebP format (named to match .blend files)
├── materials.json    # Structured JSON dataset cataloging all materials
└── README.md
```

- **[`blend-files/`](https://github.com/Infinitode/Material-Library/blob/main/blend-files)**: Contains all individual `.blend` files for every material in the library. You can append or link these materials directly into your Blender projects.
- **[`materials/`](https://github.com/Infinitode/Material-Library/blob/main/materials)**: Contains WebP preview renders for each material. Images are named identically to their corresponding `.blend` file (e.g., `deformed-metal-1.webp` corresponds to `deformed-metal-1.blend`).

## Metadata (`materials.json`)

The [`materials.json`](https://github.com/Infinitode/Material-Library/blob/main/materials.json) file catalogs all available materials in the library in a structured format, enabling web apps, add-ons, or external tools to query and display the material index.

### Format

```json
[
  {
    "image": "deformed-metal-1.webp",
    "name": "Deformed Metal 1",
    "blend-file": "blend-files/deformed-metal-1.blend"
  }
]
```

### Properties Description

| Field        | Type     | Description                                                                |
| :----------- | :------- | :------------------------------------------------------------------------- |
| `image`      | `string` | The filename of the WebP preview image located in the `materials/` folder. |
| `name`       | `string` | The human-readable display name of the material.                           |
| `blend-file` | `string` | Relative filepath to the downloadable `.blend` file.                       |

## Links

- **Website**: [Infinitode Material Library](https://infinitode.netlify.app/resources/material-library)

## License

MIT
