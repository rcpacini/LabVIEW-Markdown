# Markdown


## Examples

### Markdown.lvlib : Example.vi

Open and run the `Example.vi` to see an how to export a LabVIEW Library (*.lvlib) to markdown documentation.

This is useful to autogenerate API help documentation for GitHut.

![%demo_name%](markdown/Example_Markdown.lvlib_Example.vi.png)



## VI Tree

Markdown contains three sections:
- <b>Examples</b> - Example VIs
- <b>API</b> - Top level VIs
- <b>SubVIs</b> - Low level VIs

**Examples**

![Examples](markdown/Palette_Examples.png)

**API**

![API](markdown/Palette_API.png)

**SubVIs**

![SubVIs](markdown/Palette_SubVIs.png)



## VI Descriptions

**API**

---

### Markdown.lvlib : Markdown Library.vi

![Markdown.lvlib : Markdown Library.vi](markdown/Markdown.lvlib_Markdown_Library.vi.png)

Exports a LabVIEW Library (*.lvlib) to markdown help documentation.

Markdown template:

```
# <library_name>
<library_description>

## Examples
<example_vi_description>

## VI Tree
<vi_tree_description>
<palettes>

## VI Descriptions
### <VI>
<vi_conpane_image>
<vi_description>
```

**SubVIs**

---

### Markdown.lvlib : Close.vi

![Markdown.lvlib : Close.vi](markdown/Markdown.lvlib_Close.vi.png)

Return the exported markdown and images paths and close the library references.

### Markdown.lvlib : ConPanes.vi

![Markdown.lvlib : ConPanes.vi](markdown/Markdown.lvlib_ConPanes.vi.png)

Exports the VI connector pane images.

### Markdown.lvlib : Exmples.vi

![Markdown.lvlib : Exmples.vi](markdown/Markdown.lvlib_Exmples.vi.png)

Exports the example VIs (i.e. Starts with "Example*.vi") block diagram images.

### Markdown.lvlib : Global.vi

![Markdown.lvlib : Global.vi](markdown/Markdown.lvlib_Global.vi.png)

Markdown global variables. This library uses a global variable to avoid large data flow copies.

### Markdown.lvlib : Image Fill.vi

![Markdown.lvlib : Image Fill.vi](markdown/Markdown.lvlib_Image_Fill.vi.png)

Flood connector pane and icon 24-bit images to mask white (255, 255, 255).

### Markdown.lvlib : Load.vi

![Markdown.lvlib : Load.vi](markdown/Markdown.lvlib_Load.vi.png)

Load the library project references.

### Markdown.lvlib : Open.vi

![Markdown.lvlib : Open.vi](markdown/Markdown.lvlib_Open.vi.png)

Initialize the markdown generator, resets the global variables and resolves the markdown paths.

Use `%name%` to replace the Library name (without extension) in the output filepaths.

### Markdown.lvlib : Palette Draw.vi

![Markdown.lvlib : Palette Draw.vi](markdown/Markdown.lvlib_Palette_Draw.vi.png)

Draw diagram palette images as "text and image".

### Markdown.lvlib : Palette Grid.vi

![Markdown.lvlib : Palette Grid.vi](markdown/Markdown.lvlib_Palette_Grid.vi.png)

Returns the VI Tree palette positions based on the decorations. This calculates the grid positions by alignment on the VI Tree block dragram.

### Markdown.lvlib : Palettes.vi

![Markdown.lvlib : Palettes.vi](markdown/Markdown.lvlib_Palettes.vi.png)

Export palette images from the VI Tree SubVI positions on the block diagram. Use a square decoration to create sub-palettes.

### Markdown.lvlib : Render.vi

![Markdown.lvlib : Render.vi](markdown/Markdown.lvlib_Render.vi.png)

Render the Library markdown.

**TypeDefs**

---

### Markdown.lvlib : Item.ctl

![Markdown.lvlib : Item.ctl](markdown/Markdown.lvlib_Item.ctl.png)

Library item information.


