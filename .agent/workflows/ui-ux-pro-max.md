---
description: UI/UX design intelligence. 50 styles, 21 palettes, 50 font pairings, 20 charts, 8 stacks. Actions: design, build, create, review, fix UI/UX.
---

# UI/UX Pro Max - Design Intelligence

Searchable database of UI styles, color palettes, font pairings, chart types, product recommendations, UX guidelines, and stack-specific best practices.

## Prerequisites

Ensure Python is installed:
```bash
python3 --version
```
(Install via `brew install python3` on macOS if missing)

## How to Use This Workflow

When you need to design, build, review, or improve UI/UX:

### Step 1: Analyze Requirements
Identify: **Product type**, **Style keywords**, **Industry**, **Stack**.

### Step 2: Search Domain Knowledge
Use `run_command` to execute the search script.
**Script Path**: `.agent/resources/ui-ux-pro-max/scripts/search.py`

**Command Template**:
```bash
python3 .agent/resources/ui-ux-pro-max/scripts/search.py "<keyword>" --domain <domain> [-n <max_results>]
```

**Recommended Search Flow**:

1.  **Product** (Style recs):
    ```bash
    python3 .agent/resources/ui-ux-pro-max/scripts/search.py "saas dashboard" --domain product
    ```

2.  **Style** (Detailed guides):
    ```bash
    python3 .agent/resources/ui-ux-pro-max/scripts/search.py "minimal dark" --domain style
    ```

3.  **Typography** (Font pairings):
    ```bash
    python3 .agent/resources/ui-ux-pro-max/scripts/search.py "modern clean" --domain typography
    ```

4.  **Color** (Palettes):
    ```bash
    python3 .agent/resources/ui-ux-pro-max/scripts/search.py "tech blue" --domain color
    ```

5.  **UX** (Best practices):
    ```bash
    python3 .agent/resources/ui-ux-pro-max/scripts/search.py "accessibility" --domain ux
    ```

### Step 3: Stack Guidelines
Default is `html-tailwind`. Specify stack for specific best practices.

```bash
python3 .agent/resources/ui-ux-pro-max/scripts/search.py "layout" --stack html-tailwind
```

Available stacks: `html-tailwind`, `react`, `nextjs`, `vue`, `svelte`, `swiftui`, `react-native`, `flutter`

---

## Reference: Available Domains

| Domain | Use For | Example Keywords |
|--------|---------|------------------|
| `product` | Product type recommendations | SaaS, e-commerce, portfolio |
| `style` | UI styles, colors, effects | glassmorphism, minimalism |
| `typography` | Google Fonts pairings | elegant, playful, modern |
| `color` | Color palettes | fintech, beauty, dark |
| `landing` | Page structure | hero, pricing, testimonials |
| `chart` | Chart types | trend, comparison, pie |
| `ux` | UX patterns & a11y | animation, z-index, loading |
| `prompt` | AI prompts & CSS | (style name) |

## Pre-Delivery Checklist

Before finishing a task, verify:
- [ ] No emoji icons (use SVG)
- [ ] `cursor-pointer` on interactives
- [ ] Hover states defined
- [ ] Light/Dark mode contrast checks
- [ ] Responsive layout (320px - 1440px)
