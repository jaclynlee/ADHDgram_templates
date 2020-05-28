# ADHDgram template

This is the basic template for the _ADHDgram_.

## Sending the monthly newsletter
Important steps to remember when sending an _ADHDgram_:
1. Update volume information under header image
2. Update TOC
3. Update links to hosted version

## Adding new sections
Main body sections are structured as follows, from the outermost container to the innermost:
1. Table row with descriptive ID
    * e.g. introLetterRow, patreonCTARow
2. Table cell
3. Table with class bodyContentBlockInner
4. Table row with id property that helps identify content
    * e.g. introLetter, patreonCTA
5. Table cell with class textContentContainer

### Single-column section

```html
<tr id="articleTopicRow"> <!-- begin [article topic] section -->
  <td>
    <table class="bodyContentBlockInner">
      <tr id="descriptionOfContent">
        <td class="textContentContainer">
          <h2>This is a header</h2><br />
            <p>This is where your body text goes.</p>
        </td> <!-- end textContentContainer -->
      </tr>
    </table> <!-- end bodyContentBlockInner -->
  </td>
</tr> <!-- end [article topic] section -->
```

## Decorative elements

### Images

By default, all images used in article sections should receive the class `standardArticleGraphic`. Image formatting should not be handled piecemeal.

### Horizontal divider
Horizontal divider code should be placed within the bodyContentBlockInner table.
```html
<tr> <!-- begin divider -->
  <td class="dividerBlockInner">
    <hr class="dividerElement" />
  </td>
</tr> <!-- end divider -->
```
