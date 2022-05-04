# FixDynamicPlaceholders
This repository is useful for fix dynamic placeholder issue after Sitecore upgrade
As we all know Sitecore 9 supports Dynamic Placeholders OOTB and does not require the third party **Dyanmic placeholder Module**. The format used by Sitecore for the dynamic placeholders is different then the format used by the Dynamic Placeholder module

Old dynamic placeholder module pattern: placeholderName_renderingId. Example:

main_d9fb20a6-0538-479b-853c-0d3290a9d610

Sitecore placeholder pattern: {placeholder key}-{rendering unique suffix}-{unique suffix within rendering}. Example:

main-{d9fb20a6-0538-479b-853c-0d3290a9d610}-0

To resolve this issue we will have to update our presentation details for these differences otherwise the renderings will not be shown on the page. To resolve this problem i created a aspx page that will update all items. 
