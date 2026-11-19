# AKC-PTARC — Design & Accessibility Justification Brief

---

### 1. The 60-30-10 Color Architecture

To eliminate visual parity with CVR Labs while respecting the zero-DOM-change constraint, we deployed the **60:30:10 rule**:

* **60% Base (`#FFFFFF` / `#F8FAFC`):** Clinical cleanroom white that replaces dull commodity-lab gray, providing spaciousness and maximum readability.
* **30% Structure (`#2B7EC0`):** Primary brand blue for headers, nav, and banners, representing scientific polymer engineering and trust.
* **10% Accent (`#CF3438`):** Heritage UFlex red reserved **strictly for micro-focal points** (step numbers, category icons, section tags).

---

### 2. Why the Footer Changed to `#373435` (Logo Basement Anchor)

* **Logo Alignment:** The AKC-PTARC brand logo text and base plate are anchored in **Charcoal Black (`#373435`)**.
* **Brand Differentiation:** CVR Labs uses a generic corporate navy (`#081D33`). Changing the footer to `#373435` directly roots the footer in AKC's authentic logo palette rather than borrowing CVR's navy.
* **Visual Grounding:** Paired with pure white typography and a 3px `#2B7EC0` top accent line, it gives the page an authoritative, solid foundation with an exceptional **12.3:1 contrast ratio (WCAG AAA)**.

---

### 3. WCAG Accessibility Justification for Red (`#CF3438`)

| WCAG Principle | Technical Implementation | Compliance Result |
| :--- | :--- | :---: |
| **1.4.3 Contrast Ratio** | Red on White (`#FFFFFF`) achieves **5.00:1** (requires $\ge$ 4.5:1). | **PASSES (Level AA)** |
| **Strict Prohibition** | Red is **never used on blue banners** (which only gave 1.15:1; banner text is now pure `#FFFFFF`). | **PASSES (Zero Failures)** |
| **1.4.1 Non-Reliance on Color** | Every red step number (`1`, `2`, `3`) and icon is paired with explicit text labels and elevation hover states. | **PASSES** |
| **Sensory Comfort** | Restricted to $< 10\%$ surface area with all glowing drop shadows removed to prevent visual vibration and cognitive alarm. | **PASSES** |

---

### Key Takeaway for the Committee
> *"AKC's palette directly mirrors its logo identity: anchored by the logo's charcoal basement (`#373435`) and polymer blue (`#2B7EC0`), with accent red (`#CF3438`) mathematically certified under WCAG Level AA (5.0:1) and strictly capped at 10% to ensure clinical authority without sensory fatigue."*
