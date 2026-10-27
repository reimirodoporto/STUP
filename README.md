# Space Travelers Universal Playlist
### Core Algorithm & Predictor Engine (v11.0)

> A decoupled Tampermonkey userscript and algorithmic framework utilizing Golden Ratio ($\Phi$) grid weights, a ternary intent state machine, and Hugging Face dataset telemetry ingestion for harmonic signal analysis.

---

## 🌌 Overview

**Space Travelers Universal Playlist** is an experimental userscript engine built around the **Span of Zero** paradigm. It decouples data ingestion from non-linear algorithmic processing, allowing real-time telemetry analysis, trailing-three predictor evaluation, and checksum receipt validation across a 121-node harmonic grid.

---

## 📐 Core Architecture

The architecture is divided into two distinct zones:

### 1. Predictor Zone (`PredictorZone`)
* **Dataset Ingestion:** Automatically fetches benchmark telemetry rows from the Hugging Face datasets server (`spanofzero/SpaceTravelersUniversalPlaylist`).
* **Trailing Predictor Analysis:** Evaluates indices 117, 118, and 119 to derive the step velocity delta leading up to the 120-node boundary split.
* **Fallback Buffer:** Seamlessly falls back to local signal arrays if network restrictions apply.

### 2. Core Algorithm Engine (`CoreAlgorithmEngine`)
* **121-Node Harmonic Grid:** Non-linear harmonic weights scaled via mass attenuation and the Golden Ratio ($\Phi = 1.618033988749895$).
* **Ternary Intent State Machine:** Categorizes operational states into three discrete domains (`-1`, `0`, `1`).
* **ROM Checksum Validation:** Generates and validates cryptographic-style receipts across a $60 \times 60$ matrix space anchored by Node 120 (`||`).

---

## 🧮 Mathematical & Structural Foundation

| Component | Formula / Mechanism | Description |
| :--- | :--- | :--- |
| **Golden Ratio ($\Phi$)** | $1.618033988749895$ | Fundamental scaling factor applied across node resonance weights. |
| **Mass Attenuation** | $1.0 - (i / \text{NODES})$ | Decays harmonic weight intensity progressively across the 121 nodes. |
| **Velocity Delta** | $(signal[119] - signal[117]) / 2.0$ | Evaluates the trajectory slope across trailing predictor indices. |
| **Ternary Threshold** | $\lvert \Delta \rvert > 0.618$ | Determines whether the engine operates in historical, central, or pre-deterministic territory. |

---

## 🔌 API Documentation

Once loaded in the browser, the engine exposes a unified global API via `window.SpaceTravelersPlaylist` (and `unsafeWindow.SpaceTravelersPlaylist`):

### Methods

* **`compute(signal)`**
  * *Parameters:* `signal` (Array of numbers)
  * *Returns:* `Number` (Resonance score)
  * *Description:* Computes the weighted harmonic resonance across the input signal.

* **`analyze(signal)`**
  * *Parameters:* `signal` (Array of numbers)
  * *Returns:* `String` (Diagnostic text report)
  * *Description:* Extracts trailing predictors, evaluates the ternary state, and renders the 121-node grid diagnostic map.

* **`generateReceipt(a, b, c)`**
  * *Parameters:* `a` (Number), `b` (Number), `c` (Number)
  * *Returns:* `String` (Generated receipt string, e.g., `0A`)
  * *Description:* Computes a checksum receipt using the internal $60 \times 60$ ROM matrix.

* **`validateReceipt(receipt, a, b, c)`**
  * *Parameters:* `receipt` (String), `a`, `b`, `c` (Numbers)
  * *Returns:* `String` (Validation status message)
  * *Description:* Validates whether a given receipt matches the expected allocation parameters.

---

## 🚀 Installation & Quickstart

1. Install a userscript manager extension such as **Tampermonkey** or **Violentmonkey** in your browser.
2. Create a new userscript and paste the contents of `space-travelers-engine.user.js`.
3. Save the script and open any webpage.
4. Open your browser's Developer Console (`F12`) and interact with the engine:

```javascript
// Run a diagnostic analysis with a sample signal array
const sampleSignal = Array.from({ length: 121 }, () => Math.random());
console.log(SpaceTravelersPlaylist.analyze(sampleSignal));

// Compute resonance
const resonance = SpaceTravelersPlaylist.compute(sampleSignal);
console.log("Resonance Score:", resonance);

// Generate and validate a receipt
const receipt = SpaceTravelersPlaylist.generateReceipt(12, 34, 56);
console.log(SpaceTravelersPlaylist.validateReceipt(receipt, 12, 34, 56));
