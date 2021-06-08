# Migration guide
- 2.0+ Introduced plugin system, grouping, sorting and filtering.
- 3.0+ Breaking changes introduced:
    - Removed viewport component, this extra layer was redundant;
    - Changed classes to complex names in order to support bootstrap and other libraries:
        - row -> rgRow;
        - col -> rgCol;
        - data-cell -> rgCell;
        - data-header-cell -> rgHeaderCell;
    - All methods migrated to lowercase in order to support the modern approach of event naming. It means events name migration: `afterEdit` -> `afteredit` for all events. Check api for details;
    - Added pure esm modules support in order to use the grid in all modern frontend tooling like vitejs, parcel etc, now you can import custom-elements without lazy loading, just keep in mind you are responsible for polifills.