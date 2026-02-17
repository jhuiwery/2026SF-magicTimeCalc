# 🎩 Time Freeze Magic Calculator (2026 Spring Festival Edition)

[中文文档](README_CN.md) | [Live Demo](#) <!-- You can add a GitHub Pages link here later -->

A pixel-perfect web reproduction of the **"Time Freeze"** magic trick performed by Deng Nanzi at the **2026 CCTV Spring Festival Gala**.

This project recreates the calculator prop used in the magic show using HTML, CSS, and JavaScript. It features an iOS-style interface, responsive design (Card view on PC, Fullscreen on Mobile), and the core mathematical logic to "predict" the current time.

## ✨ Features

*   **1:1 iOS UI**: Identical look and feel to the native iOS calculator, including active states and layout.
*   **Responsive Design**:
    *   **Mobile**: Full-screen immersive experience (looks like a real app).
    *   **PC**: Displayed as a mobile phone container (Card style) with a blurred background.
*   **Magic Logic**:
    *   **Step 1**: Requires exactly **4 digits** input.
    *   **Step 2**: Requires exactly **5 digits** input.
    *   **Step 3 (The Trick)**: Any key press visually inputs a number, but logically calculates the difference needed to sum up to the current system time.
*   **Time Synchronization**: Real-time calculation ensures the result matches the exact moment the `=` button is pressed. Includes a **20-second threshold** (xx:xx:40) to auto-advance to the next minute for safety.

## 🚀 How to Use (Magic Routine)

1.  **Preparation**: Open the `index.html` on your phone (Add to Home Screen for best results).
2.  **Step 1**: Ask a spectator to input a **4-digit** number (e.g., birth year) and press `+`.
3.  **Step 2**: Ask another spectator to input a **5-digit** number and press `+`.
4.  **Step 3**: Turn the phone over or look away, and randomly tap numeric keys to "generate chaos".
    *   *Secret*: The code intercepts these taps and inputs the pre-calculated number required to force the result.
5.  **Finale**: Press `=` to reveal the sum. The result will be a 7-digit number representing the current date and time (e.g., `2162227` = Feb 16th, 22:27).

## 🛠 Technical Details

*   **No Dependencies**: Pure HTML5, CSS3, and Vanilla JavaScript.
*   **Input Validation**: Strict enforcement of 4-digit and 5-digit inputs for the first two steps.
*   **Dummy Buttons**: Buttons like `÷`, `×`, `-`, `%`, `±` have visual feedback but no logical function, preventing calculation errors during the performance.

## ⚠️ Disclaimer & Notes

1.  **Not a Real Calculator**: This is a magic prop. Standard arithmetic functions are disabled.
2.  **Sequence is Key**: You must follow the "4-digit -> 5-digit" sequence.
3.  **System Time**: The result depends on the device's system time. Ensure your clock is accurate before performing.
4.  **Pro Mode**: You can hide the top "Instruction Bar" by setting `.magic-tip { display: none; }` in the CSS for a more convincing effect.

## 📄 License

MIT License. Feel free to use this for learning or performance!
