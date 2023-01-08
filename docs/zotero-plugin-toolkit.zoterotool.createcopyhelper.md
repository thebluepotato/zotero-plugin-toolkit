<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [zotero-plugin-toolkit](./zotero-plugin-toolkit.md) &gt; [ZoteroTool](./zotero-plugin-toolkit.zoterotool.md) &gt; [createCopyHelper](./zotero-plugin-toolkit.zoterotool.createcopyhelper.md)

## ZoteroTool.createCopyHelper() method

create a `CopyHelper` instance for text/rich text/image

<b>Signature:</b>

```typescript
createCopyHelper(): CopyHelper;
```
<b>Returns:</b>

CopyHelper

## Example 1

Copy plain text

```ts
const tool = new ZoteroTool();
tool.getCopyHelper().addText("plain", "text/unicode").copy();
```

## Example 2

Copy plain text &amp; rich text

```ts
const tool = new ZoteroTool();
tool.getCopyHelper().addText("plain", "text/unicode")
                    .addText("<h1>rich text</h1>", "text/html")
                    .copy();
```

## Example 3

Copy plain text, rich text &amp; image

```ts
const tool = new ZoteroTool();
tool.getCopyHelper().addText("plain", "text/unicode")
                    .addText("<h1>rich text</h1>", "text/html")
                    .addImage("data:image/png;base64,...")
                    .copy();
```
