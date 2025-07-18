# Sub File 1
2. Contents That Might "Break" or Challenge Functionality
If you're testing DevRev's or any system’s ability to parse or render .md files properly (e.g., for robustness, edge case handling), try including:

A. 🧪 Complex / Edge Markdown Syntax
Nested lists with inconsistent indentations

Improperly closed code blocks

Mixed inline and block-level HTML

Unescaped characters: <, >, &, *, etc.

B. 🧪 Large Content or Repetition
Extremely large .md files (e.g., 10,000+ lines)

Repeated headings or sections

Overuse of the same formatting (e.g., 500 checkboxes)

C. 🧪 Encoding / Non-Standard Characters
Emojis, special unicode: 😀, ©, π, 汉字

Non-breaking spaces (\u00A0)

Right-to-left languages (Arabic, Hebrew)

Invisible characters (zero-width space \u200B)

D. 🧪 Embedded Content
Inline HTML (e.g., <script>, <style>, <iframe>)

Base64 images:
![img](data:image/png;base64,...)

E. 🧪 Invalid Markdown
Broken image or link syntax

Unescaped HTML tags that might be misinterpreted as code

Mismatched or unclosed tags/code blocks

