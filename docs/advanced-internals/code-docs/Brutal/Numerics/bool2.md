<sub><sup>Tested with: **KSA Version 2025.11.4.2791**</sup></sub>
# struct Brutal.Numerics.bool2
> **Namespace:** `Brutal.Numerics`  
> **Assembly:** `Brutal.Core.Numerics.dll`


Represents a pair of booleans.

## Constructors

### `bool2(bool x, bool y)`

Creates a `bool2` from two explicit boolean values.

* Parameters

  * `x` — Value for the `X` component
  * `y` — Value for the `Y` component

---

### `bool2(bool value)`

Creates a `bool2` where both components (`X` and `Y`) are set to the same boolean value.

* Parameters

  * `value` — The boolean assigned to both components

---

### `bool2(ReadOnlySpan<bool> span)`

Creates a `bool2` from the first two elements of a `ReadOnlySpan<bool>`.

* Parameters

  * `span` — A span containing at least two boolean values

---

### `static bool2 Load(in ReadOnlySpan<bool> span)`

Creates a `bool2` from a span, equivalent to calling the span constructor.

* Parameters

  * `span` — A read-only span containing the values

## Members

### Fields

#### `bool X`

The X component of the vector.
XML-serializable.

#### `bool Y`

The Y component of the vector.
XML-serializable.

---

### Indexer

#### `bool this[int index]`

Gets or sets a component by index.

* 0 → X
* 1 → Y

Throws on out-of-range indices.

---

### Static Properties

#### `int ComponentSize`

The size of each component in bytes. Always `1`.

#### `int Count`

The number of components in the vector. Always `2`.

#### `bool2 Zero`

A `bool2` with both components set to `false`.

#### `bool2 One`

A `bool2` with both components set to `true`.

#### `bool2 UnitX`

A vector where `X = true`, `Y = false`.

#### `bool2 UnitY`

A vector where `X = false`, `Y = true`.

---

### Swizzle Properties

#### `bool2 XY`

Gets or sets the vector as `(X, Y)`.

#### `bool2 YX`

Gets `(Y, X)` or sets by reversing assignment order.

#### `bool R`

Alias for component `X`. (Red)

#### `bool G`

Alias for component `Y`. (Green)

#### `bool2 RG`

Alias for `(R, G)` same as `(X, Y)`.

#### `bool2 GR`

Alias for `(G, R)` same as `(Y, X)`.

---

## Methods

#### `void Deconstruct(out bool x, out bool y)`

Deconstructs the vector into two variables.

---

### `Span<bool> AsSpan()`

Returns a span referencing the two component values.

---

### `void CopyTo(bool[] array)`

Copies the components into an array starting at index 0.
Array must be length ≥ 2.

### `void CopyTo(bool[] array, int index)`

Copies the components into an array starting at a specific index.

### `void CopyTo(Span<bool> destination)`

Copies the components into a span.
Must have length ≥ 2.

### `bool TryCopyTo(Span<bool> destination)`

Attempts to copy the components.
Returns `false` if the destination span is too small.

---

### `bool Length()`

Returns whether the vector has any `true` component.
Equivalent to OR-ing all elements.

### `bool LengthSquared()`

Same as `Length()`.
Returns `Y` if `X` is false, else `true`.

---

### `static bool2 Load(in ReadOnlySpan<bool> span)`

Creates a `bool2` from the first two elements of a span.

---

### `override int GetHashCode()`

Returns a combined hash of both components.

### `bool Equals(bool2 other)`

Checks component-wise equality.

### `override bool Equals(object? obj)`

Determines whether the object is a `bool2`.

---

### `string ToString()`

Returns a culture-aware formatted string for the vector.

### `string ToString(string? format)`

Formats the vector using the specified numeric format.

### `string ToString(string? format, IFormatProvider? provider)`

Formats using the given culture or provider.

---

## Operators

### Equality Operators

#### `bool operator ==(bool2 left, bool2 right)`
#### `bool operator !=(bool2 left, bool2 right)`

### Boolean Operators

#### `bool2 operator |(bool2 a, bool2 b)` — Componentwise OR
#### `bool2 operator &(bool2 a, bool2 b)` — Componentwise AND

