# markdown-to-obsidian-math-converter

This is a simple, responsive web tool that converts LaTeX-style math expressions to Obsidian-compatible math syntax. Specifically, it converts:

- Inline math expressions from `\(...\)` to `$...$`
- Block math expressions from `\[...\]` to `$$...$$`

Additionally, the tool performs a basic validity check for balanced dollar signs and provides a scrollable output area with a copy-to-clipboard feature.

## Features

- **LaTeX to Obsidian Conversion:**  
  Automatically replaces:
  - `\(...\)` with `$...$`
  - `\[...\]` with `$$...$$`

- **Validity Check:**  
  A naive check that verifies if the resulting text has balanced `$` or `$$` delimiters.

- **Responsive Design:**  
  The layout adapts to different screen sizes with a centered container and a responsive width.

- **Scrollable Output:**  
  The converted text output area is scrollable for longer texts.

- **Copy to Clipboard:**  
  Easily copy the converted text to your clipboard with the provided **Copy** button.

## How to Use

1. **Open the HTML file:**  
   Open `index.html` (or the file name you choose) in your favorite web browser.

2. **Enter your Markdown text:**  
   Paste or type your text with LaTeX math expressions in the input textarea.

3. **Convert:**  
   Click the **Convert** button to perform the conversion and check the validity of the math expressions.

4. **View Output:**  
   The converted text will appear in the scrollable output area below.

5. **Copy:**  
   Click the **Copy** button to copy the converted text to your clipboard.

## Example

**Input:**

```latex
This is inline math: \( e^{i\theta} = \cos \theta + i \sin \theta \).

This is block math:
\[
  \begin{vmatrix}
    a & b \\
    c & d
  \end{vmatrix} = ad - bc
\]
```
**Output**
```
This is inline math: $ e^{i\theta} = \cos \theta + i \sin \theta $.

This is block math:
$$
  \begin{vmatrix}
    a & b \\
    c & d
  \end{vmatrix} = ad - bc
$$
```
