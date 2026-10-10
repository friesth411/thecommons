# Project notes

Reviewed against the standalone prototype source and public tool pages on October 10, 2026.

## FrictionIndex

The standalone implementation accepts named workflows, weekly hours, an hourly rate, and an assumed percentage of friction absorbed. It scores Ingest, Switch, Drag, Rewrite, and Guides, then averages workflow scores for an organization score.

Each dimension contributes up to 20 points. Switch uses a 0–10 input range; the other inputs use 0–5. Although the interface describes Switch as double-weighted, the normalized calculation gives every dimension the same maximum contribution. Treat that wording as an implementation question to resolve before claiming a validated weighting method.

The comparison chart contains fixed example squad scores. They are demonstration data, not measured customer benchmarks. The estimated freed-value calculation depends on the entered hours, hourly rate, and assumed reduction; it is not evidence of realized cash savings.

The public calculator has a different intake flow, starting with work-week length. Its current interface should be evaluated separately from this standalone version.

## Human-Owned Zones Mapper

The standalone implementation organizes workflows or agents into HITL, HOTL, AUTO, and STOP zones, captures blast radius and a compliance gate, and exports a Markdown protocol.

The public workspace uses team context, role selection, boundary cards, and gate confirmations. Its boundary cards distinguish AI scope, human ownership, and an audit rule. Export completion requirements are visible in the interface.

A completed form records stated boundaries. It does not independently enforce those boundaries, certify compliance, or prove that review happens in practice.

## AI ROI Canvas

The standalone implementation contains eight role examples: Finance, IT Service Delivery, Project Delivery / PMO, Human Resources, Legal, Sales Operations, Marketing, and Customer Success.

The task model estimates labor capacity value, deducts token costs, and then deducts a shared human-review cost to calculate its displayed true-net figure. Human-review cost uses minutes per output, output volume, and an hourly rate.

This version does not establish a complete total-cost model. Subscription fees, integration, training, maintenance, and error consequences need separate consideration before making an investment decision. Embedded model-price hints and performance percentages are example assumptions, not verified current prices or industry findings.

The public Canvas overview is part of the Academy's membership offering. It is not presented here as a freely accessible deployment of the standalone code.

## A useful next validation

Use one workflow with an owner and a baseline. Record the time needed to prepare inputs, generate output, review it, correct it, and finish the task. Track quality and the resulting business outcome alongside time. Compare the full workflow before and after the change.

The repository review confirmed implementation features. It did not exercise the public interfaces end to end or establish customer outcomes.

## Related open notes

- [Sample HOZ protocol](../examples/sample-hoz-protocol.md)
- [Friction dimension notes](../examples/friction-dimension-notes.md)
