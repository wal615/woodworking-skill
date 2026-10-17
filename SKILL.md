# US Woodworking Design

## Start from actual dimensions, never nominal

- Convert every nominal size to its actual size before you design anything. A 2x4 is 1.5 by 3.5 in, a 4x4 is 3.5 by 3.5 in, a 1x8 is 0.75 by 7.25 in. The full table lives in references/lumber.md.

- Do all arithmetic in actual dimensions. Inner spans, insets and clearances all come from the real numbers, so a part computed from nominal sizes will not fit.

- Tell the user which sizes are nominal and which are actual whenever you present a dimension. One confused number at the lumber yard wastes a trip.

## Choose joinery for the load and the tools

- Match the joint to the load. Butt joints with screws carry light loads, lag bolts or carriage bolts carry shear and racking, pocket holes hide fasteners in casework. Details are in references/joinery-and-fasteners.md.

- Prefer mechanical fasteners over glue when the piece will take pounding, vibration or disassembly. Glue is strong but permanent and unforgiving of mistakes.

- Drill pilot holes for every lag bolt and for screws near board ends. A split board ruins more than the hole. Pilot sizes are in references/joinery-and-fasteners.md.

- Put a washer under every bolt head and nut, and add a spring washer where vibration can loosen nuts.

## Write the cut list, then the cut diagram

- List every part with actual dimensions, quantity and which stock it comes from. Count twice, because one missing part stops a build day.

- Lay the parts onto the stock on paper before cutting. Group same-length cuts, keep a small kerf allowance, and mark which cuts need a flip (any cut deeper than the saw reaches in one pass).

- Draw the cut diagram as SVG or HTML you write yourself, with every label computed from the spec. Use the precise_diagrams skill for this and never use image generation for dimensioned plans.

## Draw the build views

- Give the user at least a front view and a side view, plus a top-down layout when part positions matter. Add a close-up detail for any joint that is hard to picture.

- Show fastener positions on the views, not just in a list. A dot where each bolt goes prevents the most common assembly mistake.

- Keep the editable source so revisions start from it instead of from a rendered copy.

## Build the shopping list

- Separate lumber from hardware. For lumber name the grade (#2 is fine for shop furniture), the treatment (kiln-dried, not green pressure-treated, for indoor pieces) and the count.

- For hardware give the exact size and the quantity of complete sets (bolt plus washer plus nut), not just the bolt.

- Tell the user how to pick boards at the store: sight down the length for bow and twist, reject the worst of the pile, and buy one spare of the cheapest critical part.

## Available connectors

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.

- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Websites

- [Home Depot](https://www.homedepot.com/) for checking lumber dimensions, grades and hardware availability at the user's store. Search results never confirm price or stock, so verify on the product page.

## Alternatives for better results

- Ask for the missing measurement instead of inventing it. One clarified number beats a corrected plan.

- Offer a printable version of the plans when the user will carry them to the garage or the store.

- Suggest a cheaper or simpler joint when the user's tools cannot make the first choice cleanly.
