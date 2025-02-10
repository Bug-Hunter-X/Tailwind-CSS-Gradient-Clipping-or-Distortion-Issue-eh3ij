# Tailwind CSS Gradient Rendering Bug

This repository demonstrates a bug where Tailwind CSS gradients don't render correctly when combined with certain layout or size classes.  The gradient may be clipped or distorted, resulting in an unexpected visual appearance.

## Bug Description

When using Tailwind's gradient classes (e.g., `bg-gradient-to-r`) along with classes that affect the element's dimensions (like `w-full`, `h-screen`, or padding classes), the gradient might not render as expected. It could be clipped or appear distorted.

## Reproduction

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe the unexpected rendering of the gradient.

## Solution

The solution involves carefully considering the order and combination of classes.  Sometimes explicitly setting dimensions (e.g., using `width` and `height` instead of percentage-based classes) can help. Refer to `bugSolution.html` for a corrected version.