# github-without-copilot-css
Simple CSS ruleset to stop GitHub from showing Copilot everywhere.

## How to use it

1. Install the Stylus extension or an alternative
2. Create a new rule for `github.com` and copy&paste the following ruleset
   
```css
.search-query-builder .QueryBuilder-ListWrap > li:last-child,
.CopilotWorkspaceButton-module__buttonGroup--ZEfG8, .CopilotWorkspaceButton-module__buttonGroup--ZEfG8>div:first-child,
[href="/settings/copilot"],
.AppHeader-CopilotChat.hide-sm.hide-md,
.copilotPreview__container,
[data-hovercard-type="copilot"],
[aria-controls="copilot-chat-panel"],
[data-target="copilot-diff-entry.menuItemsSlot"],
.file-diff-split .blob-code-inner+.Box-sc-g0xbh4-0.DiffLinesMenu-module__diff-button-container--UrMbh.prc-ButtonGroup-ButtonGroup-vcMeG,
.CopilotActionsChatButton-module__copilotActionsChatButton--Hb7TL.CopilotActionsChatButton-module__expanded--XgruB,
[class="octicon octicon-copilot"],
.ActionListContent:has(.octicon-copilot){
    display: none !important;
}
```

3. Enjoy.
