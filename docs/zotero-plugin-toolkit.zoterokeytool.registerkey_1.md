<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [zotero-plugin-toolkit](./zotero-plugin-toolkit.md) &gt; [ZoteroKeyTool](./zotero-plugin-toolkit.zoterokeytool.md) &gt; [registerKey](./zotero-plugin-toolkit.zoterokeytool.registerkey_1.md)

## ZoteroKeyTool.registerKey() method

Register a key using XUL element &lt;<!-- -->key<!-- -->&gt;<!-- -->.

The command might not be triggered if there are conflictions.

<b>Signature:</b>

```typescript
registerKey(type: "element", keyOptions: {
        id: string;
        key: string;
        modifiers?: keyof KeyModifierStatus;
        disabled?: boolean;
        xulData: {
            document?: Document;
            command?: string;
            oncommand?: string;
            _commandOptions?: {
                id: string;
                document: Document;
                oncommand?: string;
                disabled?: boolean;
                label?: string;
                _parentId: string;
            };
            _parentId: string;
        };
    }): boolean;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  type | "element" |  |
|  keyOptions | { id: string; key: string; modifiers?: keyof KeyModifierStatus; disabled?: boolean; xulData: { document?: Document; command?: string; oncommand?: string; \_commandOptions?: { id: string; document: Document; oncommand?: string; disabled?: boolean; label?: string; \_parentId: string; }; \_parentId: string; }; } |  |

<b>Returns:</b>

boolean

`true` for success and `false` for failure.
