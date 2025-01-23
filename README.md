# Uncommon CSS Bug: `:focus-visible` and `pointer-events: none` Conflict

This repository demonstrates an uncommon bug related to the interaction between the CSS `:focus-visible` pseudo-class and the `pointer-events: none` property.  The bug occurs when an input element nested within a container that uses `pointer-events: none` does not visually indicate focus as expected with `:focus-visible`.

This is a subtle accessibility issue as it prevents users who rely on visual focus indicators from understanding which element is currently active.

## Bug Description
The `:focus-visible` pseudo-class is designed to only apply styles when the focus is visually apparent, improving user experience. However, when the parent element uses `pointer-events: none`, the visual indication of focus can be suppressed, rendering `:focus-visible` ineffective.

## Solution
The provided solution explains how to address the problem effectively, ensuring correct focus indication even with parent elements that disable pointer events.