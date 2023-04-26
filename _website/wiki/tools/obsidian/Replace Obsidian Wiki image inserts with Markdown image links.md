%{
}
---

An image inserted with Wiki notation: `![[Image.png]]` can be inserted with Markdown notation with a relative path: `![Image](../../resources_path/Image.png)` by running a find and replace Regex in the document:

- **Find**: `!\[\[(.*)\.png\]\]`
- **Replace:** `![$1](../../../../_resources/$1.png)`