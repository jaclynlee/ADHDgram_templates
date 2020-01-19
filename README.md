# ADHDgram template

This is the basic template for the _ADHDgram_.

## Adding new sections
Main body sections are structured as follows, from the outermost container to the innermost:
1. Table cell with class templateBody
2. Table with class templateContainer
3. Table row with id property that helps identify content
..* e.g. introLetter, patreonCTA
4. Table cell with class textContentContainer

### Single-column section

```html
<td align="center" valign="top" class="templateBody">
  <table align="center" border="0" cellpadding="0" cellspacing="0" width="100%" class="templateContainer">
    <tr id="descriptionOfContent">
      <td class="textContentContainer">
            <h2 style="text-align: left;">This is a header</h2><br />
              <p>This is where your body text goes.</p>
      </td>
    </tr>
  </table>
</td>
```

## Decorative elements

### Horizontal divider
```html
<tr id="followBlockTopBorder">
  <td class="dividerBlockInner">
    <hr class="dividerElement" />
  </td>
</tr>
```
