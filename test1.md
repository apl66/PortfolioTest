<!-- This is the project decription. Here the short details of the project will be provided -->
# 🚀 Markdown Test File: Level 1 Header

This is a standard paragraph containing **bold text**, *italic text*, and `inline code`. You can also use ~~strikethrough text~~ to show edits.

## 📋 Text Elements (Level 2)

### 🧩 Lists and Blocks (Level 3)

Here is an unordered bulleted list:
* First punchy item.
* Second distinct point.
* Third fast detail.

Here is an ordered numbered list:
1. Initialize the project.
2. Configure settings.
3. Deploy to production.

> **Note:** This is a blockquote element. It is commonly used for callouts, warnings, or highlighting critical contextual details.

---

## 💻 Technical Elements

### 🛠️ Code Blocks
Below is a syntax-highlighted C# sample demonstrating string checking:

```csharp
using System;

public class Program
{
    public static void Main()
    {
        string text = "Blazor Development";
        bool containsWord = text.Contains("Blazor", StringComparison.OrdinalIgnoreCase);
        
        Console.WriteLine(\$"Contains match: {containsWord}");
    }
}
```

### 📊 Data Table

| Feature | Method | Output Type |
| :--- | :--- | :--- |
| Exists | `.Contains()` | `bool` |
| Position | `.IndexOf()` | `int` |
| Count | `.Count()` | `int` |

---

## 🔗 Media Elements

* **Hyperlink:** [Visit Microsoft .NET Documentation](https://microsoft.com)
* **Task List:**
  - [x] Create test file architecture
  - [ ] Verify UI framework rendering
  - [ ] Ship to staging environment
