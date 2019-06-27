
# Vscode vim setup 

Personalization for vim mode in VScode, for Mac. For other OS, changing the "cmd" key mappings to "ctrl" might work.

## Shortcuts 

Copy the keybindings.json into the json editor under Code -> Preferences -> Keyboard Shortcuts. 

Any existing mapping for these key combonations needs to be unmapped first. See the keybindings.json file, any mapping whose  "command" starts with "-" is an unmapping of a default shortcut. 

**Note:** To use h/j/k/l in the explorer tree,  add `"workbench.list.automaticKeyboardNavigation": false` to settings.json. Otherwise it will show the file filter/highlighting instead of navigating. 

### In keybindings.json

Keys | Action  | Vscode mapping name 
--- | --- | --- 
`"cmd+{"  "cmd+}"` | Select next/previous open editor tab | workbench.action.nextEditor or .previousEditor
"`" | Toggle sidebar (explorer) like NerdTree | workbench.action.toggleSidebarVisibility" 
`cmd + h/j/k/l` | move to pane in the direction of h/j/k/l key | workbench.action.navigateDown/Up/etc

### In settings.json - vim.normalModeKeyBindingsNonRecursive
Keys | Action  | Vscode mapping name 
--- | --- | --- 
"`" | Toggle sidebar (explorer) like NerdTree | workbench.action.toggleSidebarVisibility" 
`u, U` | undo/redo | 

