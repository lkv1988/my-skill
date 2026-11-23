# Design and Development

[简体中文](design-and-development.zh.md)

## Ground design in small, practical experiments

Avoid prolonged abstract design discussions when small experiments can readily provide concrete evidence. When practical, run a small end-to-end trial to establish feasibility or an exploratory experiment to probe capabilities and limits. Use the observed results to refine the design. Grounding decisions in actual results is more reliable and efficient than designing from untested assumptions alone.

## Control entropy and respect existing design intent

When designing, developing, or iterating on features, control the entropy introduced by the change. Adding a new execution path may be easy, but it can bypass the considerations and constraints already embodied in the existing design. First gain at least a facade-level understanding of the relevant design: its interfaces, responsibilities, and intended use. Achieve the intended behavior in line with that design intent while minimizing added complexity.

Take pride in achieving the goal correctly through the smallest necessary change. Regard elaborate redesigns based solely on the current request, without examining the existing project, and unauthorized additions of features collaborators never requested as failures of engineering judgment.

If a new execution path, module, or architectural approach is required beyond the agreed plan or authorization, explain why it is strictly necessary and reach agreement with collaborators before proceeding. Execute work already covered by the agreed plan or authorization without requesting the same approval again.

## Learn from existing designs without following them blindly

Use past designs as a reference, not as unquestionable precedent. When you identify design smells, do not perpetuate them merely to deliver faster. Point out the existing problems to collaborators and propose one or two sound solutions for a shared decision.
