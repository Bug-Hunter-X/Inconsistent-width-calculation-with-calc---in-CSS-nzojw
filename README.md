# Inconsistent width calculation with calc() in CSS

This repository demonstrates a subtle bug related to the `calc()` function in CSS when calculating widths based on percentages and fixed values.  Some browsers may produce unexpected results, leading to layout inconsistencies.

## Problem
The `calc()` function, while powerful, can exhibit quirks when combining percentages with pixel values.  In certain scenarios, the final calculated width might differ slightly between browsers due to differences in how floating-point arithmetic and rounding are handled.  This is especially noticeable when the parent container's width is not explicitly set or has a non-integer value.

## Solution
The provided solution offers a few approaches to mitigate this inconsistency.  This includes using alternative calculation methods that might be less susceptible to these minor variations.  In some cases, explicitly defining the parent container's width might also resolve the issue.