# up-password-input

A polymer input element with Material Design styling for entering and validating a password.

## Usage

    <up-password-input></up-password-input>

It may include an optional label, which by default is "Password".

    <up-password-input label="your password"></up-password-input>

### Password strength

The strength of the password is automatically calculated.
By adding the optional `strength-calculator` attribute, the strength is shown as one of
four categories: `bad`, `weak`, `good` or `strong`.

### Validation

The input can be automatically validated as the user is typing by using
the `auto-validate` and `required` attributes. For manual validation, the
element also has a `validate()` method, which returns the validity of the
input as well sets any appropriate error messages and styles.

By default the password is valid if the strength is at least `weak`. This can be
changed by setting the `min-strength-category` to `bad`, `weak`, `good` or `strong`.

    <up-password-input min-strength-category="good"></up-password-input>

The input can also be validated against another input field, by setting the `confirmation-for` attribute
to the id of the input field to match. In that case, the value of the other input field should
be valid and both values should be equal.

See `Polymer.PaperInputBehavior` for more API docs.

### Styling

See `Polymer.PaperInputContainer` for a list of custom properties used to
style this element.



