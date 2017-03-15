# floating-label

Demo version: https://russmaxdesign.github.io/floating-label/

A quick demo of a floating label.

### Outcomes

- Before any user interaction with an input, the placeholder should be visible and the label hidden
- When user focuses on the input, the placeholder should gradually fade out, the label should animate into view, colored blue, and the input's bottom border should change to blue
- As soon as the user enters a character into the input, the label should change to green, and the input's bottom border should change to green
- When focus leaves the input, the label should remain in view but change to dark gray, and the input's bottom border should return to the original light gray

### Potential issues

- The label, when present, is much smaller than normal text and could be hard to read for some users
- Depending on how and where this solution is used, he lack of visual definition for inputs could present usability issues for some users
- The labels associated with inputs appear after the input in source order. However, as the input and label are explicitly associated via "id" and "for" values, this should be acceptable for most assistive technologuies.
- In order to have the label remain visible after the user has left th form field, this solution uses the :valid CSS selector - which is [only supported by recent browsers](http://caniuse.com/#search=%3Avalid).

See [Licence information](LICENCE) for use.
