# Tailwind CSS flex-grow Bug

This repository demonstrates a bug where Tailwind's `flex-grow` utility doesn't behave as expected when the parent container has a constrained width.  The text within the paragraph overflows its container despite `flex-grow` being applied.

## Bug Description

The provided HTML uses `flex-grow` to make a paragraph expand to fill available space. However, if the parent container has a fixed or constrained width, the text within the paragraph overflows, instead of expanding to take up the available space within the container. This is inconsistent with the expected behavior of `flex-grow`.

## Reproduction

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that the text in the paragraph overflows the container even though `flex-grow` is applied to its parent div.

## Solution

The provided solution in `solution.html` solves this issue by utilizing `flex-shrink-0` on the avatar and a `min-width` on the flex container to ensure it expands to fit its content, while also preventing the avatar from shrinking.

