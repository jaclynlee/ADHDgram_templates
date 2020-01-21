# ADHDgram template

This is the basic template for the _ADHDgram_.

## Sending the monthly newsletter
Important steps to remember when sending an _ADHDgram_:
1. Update volume information under header image
2. Update TOC

## Adding new sections
Main body sections are structured as follows, from the outermost container to the innermost:
1. Table row with descriptive ID
* e.g. introLetterRow, patreonCTARow
2. Table cell with class bodyContentBlockOuter
3. Table with class bodyContentBlockInner
4. Table row with id property that helps identify content
* e.g. introLetter, patreonCTA
5. Table cell with class textContentContainer

### Single-column section

```html
<tr id="descriptiveName">
  <td align="center" valign="top" class="bodyContentBlockOuter">
    <table align="center" border="0" cellpadding="0" cellspacing="0" width="100%" class="bodyContentBlockInner">
      <tr id="descriptionOfContent">
        <td class="textContentContainer">
          <h2 style="text-align: left;">This is a header</h2><br />
            <p>This is where your body text goes.</p>
        </td>
      </tr>
    </table>
  </td>
</tr>
```

## Decorative elements

### Horizontal divider
Horizontal divider code should be placed within the bodyContentBlockInner table.
```html
<tr>
  <td class="dividerBlockInner">
    <hr class="dividerElement" />
  </td>
</tr>
```
