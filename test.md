<!-- Short Description: This text, tag, or metadata is completely hidden from the reader -->

# 🚀 Markdown Complex Rendering Test Suite

## 1. Typography & Inline Formatting

This paragraph tests basic formatting capabilities. It includes **strong emphasis**, *standard emphasis*, and ***combined bold and italic text***. We also need to test ~~strikethrough text~~, `inline code blocks`, and text containing <kbd>Ctrl</kbd> + <kbd>C</kbd> keyboard wrappers.

### Escaping Test
Here are literal characters that often break regex-based parsers: `_underscores_`, `*asterisks*`, `[brackets]`, `\backslashes\`, and HTML entities like `&amp;`, `&lt;`, and `&gt;`.

---

## 2. Advanced Nested Lists

1. This is the first main numbered item.
   * This is a bullet point nested under item 1.
   * This is another bullet point.
     1. Deeply nested numbered item A.
     2. Deeply nested numbered item B with a multi-line paragraph requirement.
        
        This paragraph is technically a child of item B, requiring proper indentation alignment from the rendering engine.
2. This is the second main numbered item.
   - [ ] Unchecked task list item.
   - [x] Checked task list item.

---

## 3. Tables with Alignment & Multi-line Truncation

| Project Name | Repository Status | Primary Language | Estimated Impact |
| :--- | :---: | :---: | ---: |
| **Blazor WebAssembly Portfolio** | `Active` | C# / Razor | +45% Engagement |
| Markdown Parser | `Pending Fix` | TypeScript | *N/A* |
| Legacy System Sync | ~~Deprecated~~ | PHP | `$0.00` |

---

## 4. Complex Blockquotes & Alerts

> **Important Architecture Note**
> Blockquotes should support multiple paragraphs natively.
> 
>> This is a nested blockquote testing deep rendering tree execution. It must inherit parent styles cleanly without overflowing horizontal container widths.
>
> Back to the primary level blockquote context block.

---

## 5. Multi-Language Code Blocks

### C# Dependency Injection Example
```csharp
using Microsoft.AspNetCore.Components;
using System.Net.Http;

namespace Portfolio.Services
{
    public class MarkdownService : IMarkdownService
    {
        private readonly HttpClient _http;
        private readonly ILogger<MarkdownService> _logger;

        public MarkdownService(HttpClient http, ILogger<MarkdownService> logger)
        {
            _http = http ?? throw new ArgumentNullException(nameof(http));
            _logger = logger;
        }
    }
}
```

### JSON Configuration Example
```json
{
  "ProjectSettings": {
    "CacheDuration": "00:30:00",
    "AllowedExtensions": [".md", ".txt", ".json"],
    "Features": {
      "EnablePrerendering": true,
      "MetricsLevel": "Verbose"
    }
  }
}
```

---

## 6. Mathematical Expressions (LaTeX)

When using parsers that include KaTeX or MathJax extensions, math blocks should compile cleanly.

An inline equation: $E = mc^2$

A block equation matrix:

$$
\begin{pmatrix}
1 & x & x^2 \\
1 & y & y^2 \\
1 & z & z^2
\end{pmatrix}
$$

---

## 7. Edge Cases & Bad Syntax Handling

* Left dangling delimiter test: **Oops, I forgot to close this bold string.
* Empty links: [Internal Reference]()
* HTML Injection Test: <div style="background-color: red; color: white; padding: 10px;">If your parser allows raw HTML, this box will be red with white text.</div>
