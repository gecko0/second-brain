# CAD Skill

## Summary

`cad-skill` is a Claude Code skill by Flowful AI for generating parametric, 3D-printable CAD models with CadQuery. It is useful when an agent needs to turn a physical-object request into a script, STL export, rendered preview, and iterative printability review.

## Key Points

- The skill targets functional 3D-printable parts such as enclosures, brackets, mounts, cases, housings, adapters, organizers, and mechanical components.
- It uses CadQuery and Python to create parametric geometry, then exports STL files for slicing.
- The intended workflow is collaborative and phased: gather requirements, research real-world dimensions when needed, build a base shape, add features, then finalize with fillets, chamfers, previews, and print recommendations.
- It includes helper scripts for running CadQuery models, rendering multi-view STL previews, validating mesh output, and converting STL to 3MF for slicers such as Bambu Studio or PrusaSlicer.
- The skill emphasizes print-friendly defaults such as clearances, wall thickness, orientation, minimum feature sizes, overhang limits, and material-specific adjustments.
- Main dependencies to remember: Python 3.10-3.12, CadQuery, trimesh, pyrender, Pillow, numpy, and lxml.
- License note: the repository uses the PolyForm Noncommercial License 1.0.0.

## Sources

- [flowful-ai/cad-skill on GitHub](https://github.com/flowful-ai/cad-skill)
- [CAD Skill README](https://raw.githubusercontent.com/flowful-ai/cad-skill/main/README.md)
- [CAD Skill SKILL.md](https://raw.githubusercontent.com/flowful-ai/cad-skill/main/SKILL.md)

## Related

- [Agent Skills](agent-skills.md)
- [drawio-skill](drawio-skill.md)
- [Resources](../../README.md)
