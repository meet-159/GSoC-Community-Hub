# Docslink Component

## Description
The `Docslink` component is a **simple and clean link separator** designed to display two clickable links side by side, separated by a vertical bar (`|`).

Useful for placing paired navigation options, such as:
- **Documentation ↔ GitHub**
- **Privacy Policy ↔ Terms of Use**
- **Previous ↔ Next** article links

---

## Usage

Use this component to visually separate two links in a clean and centered layout. Ideal for navigation footers or section dividers.

---

## Props

| Prop Name   | Type     | Default | Description                               |
| ----------- | -------- | ------- | ----------------------------------------- |
| `leftlink`  | `string` | `""`    | The text or link to display on the left.  |
| `rightlink` | `string` | `""`    | The text or link to display on the right. |


> **Note**: You can pass complete anchor tags (e.g. `<a href="/docs">Docs</a>`) to `leftlink` and `rightlink`.

---

## Example


```svelte

<script>
    const leftlink = "Read the Guides";
    const rightlink = "Read Release Notes";
</script>

use Docslink from $lib/components/docslink/Docslink.svelte

get leftlink
get rightlink

<main>

<Docslink {leftlink} {rightlink}/>

</main>

```

This example is available for build and test at [Examples](../examples/docslink.md)
---

The above code outputs a component :

![Docslink image.](./docsImages/docsLinkImage.png "This is a Docslink component image.")