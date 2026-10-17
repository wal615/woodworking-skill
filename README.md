# woodworking

A Claude skill for US woodworking design. It teaches how to design furniture
and shop projects with US dimensional lumber: actual vs nominal dimensions,
joinery and fastener choice, cut lists, hand-drawn dimensioned cut diagrams
and plans, and Home Depot shopping lists.

## Contents

- `SKILL.md` - the method: design in actual dimensions, choose joinery for the
  load, write the cut list, draw the plans, build the shopping list
- `skill.yaml` - skill metadata
- `references/lumber.md` - nominal vs actual dimension tables, sheet goods,
  grades, treatment, how to pick boards
- `references/joinery-and-fasteners.md` - joints by strength, wood screws, lag
  screws, carriage bolts, no-glue mechanical builds
- `references/cutting.md` - circular saw depth limits, the flip-cut technique,
  marking miters, basic safety

## Companion skill

Pairs with `precise_diagrams` (draw exact SVG/HTML diagrams from a spec, never
AI-generated images for dimensioned plans).

## Origin

Built from a real project: a heavy no-glue workbench (80x27x2 in top, 4x4
legs, bolted joinery) designed with its owner in October 2026.
