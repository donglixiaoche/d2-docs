# Layouts

D2 supports using a different layout engines. The choice of layout engines can
significantly influence your overall diagram.

## Layout engines

- [dagre](https://github.com/dagrejs/dagre) (default): A fast, directed graph
  layout engine that produces layered/hierarchical layouts. Based on Graphviz's DOT
  algorithm.
- [ELK](https://github.com/kieler/elkjs): Also a directed graph layout engine. More mature
  than dagre, better maintained (part-time academic research team working on it), with
  recent releases.
- [TALA](https://github.com/terrastruct/TALA): New layout engine designed
  specifically for software architecture diagrams. Requires separate install, visit the
  Github page for more, including samples.

D2 intends to integrate with a variety of layout engines, e.g. `dot`, as well as
single-purpose layout types like sequence diagrams. You can choose whichever layout engine
you like and works best for the diagram you're making.

To compare D2 renders with the various layout engines, visit
[https://text-to-diagram.com](https://text-to-diagram.com) and toggle the layout engines
in the comparison settings.

To see available layouts on your machine, you can run `d2 layout`.

To specify the layout used, you can either set the flag `--layout=dagre` or set it as an
environment variable, `$D2_LAYOUT=dagre`.