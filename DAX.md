
[Glossary](#format)





### Format

In Power BI, you can use the **DAX FORMAT function** to format numbers in the Indian numbering system (with commas for lakhs and crores). Here's how you can do it:

### DAX Formula Example:
```DAX
FormattedValue = FORMAT(SUM('Table'[Amount]), "#,##,##0")
```

### Explanation:
- `#` represents optional digits.
- `,` specifies the position of separators.
- The format `#,##,##0` applies the Indian numbering style:
  - Two digits after the first separator (for lakhs and crores).
  - Then groups of three digits for thousands.

### Example Output:
For a number like `12345678`, this format will display:
```
1,23,45,678
```

If you need additional help with variations (e.g., currency symbols or decimal places), let me know!