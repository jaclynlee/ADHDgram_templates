# ADHDgram template

This is the basic template for the _ADHDgram_.

## Sending the monthly newsletter
Important steps to remember when sending an _ADHDgram_:
1. Update volume information under header image
2. Update TOC
3. Update links to hosted version
4. Update Patron acknowledgements

## Adding new sections
Main body sections are structured as follows, from the outermost container to the innermost:
1. Table row with comment to distinguish it
    * i.e., "begin article row"
2. Table cell
3. Table with class `bodyContentBlockInner`
4. Table row
5. Table cell with class `textContentContainer`
6. h2 tag with id property corresponding to TOC anchor link

### Single-column section example

```html
<tr> <!-- begin article row -->
 <td> <!-- begin article content block -->
   <table class="bodyContentBlockInner">
     <tr> <!-- begin divider -->
       <td class="dividerBlockInner">
         <hr class="dividerElement" />
       </td>
     </tr> <!-- end divider -->
     <tr>
       <td class="textContentContainer">
         <h2 id="article-1" style="text-align: left;">Section Title</h2>
         <p>
            Body text here!
         </p>
         <p>
            Body text here!
         </p>
       </td>
     </tr> <!-- end text content row -->
   </table> <!-- end bodyContentBlockInner -->
 </td> <!-- end article content block -->
</tr> <!-- end article row -->
```

## Decorative elements

### Images

By default, all images used in article sections should receive the class `standardArticleGraphic`. Image formatting should not be handled piecemeal.

### Horizontal divider
Horizontal divider code should be placed within the `bodyContentBlockInner` table.
```html
<tr> <!-- begin divider -->
  <td class="dividerBlockInner">
    <hr class="dividerElement" />
  </td>
</tr> <!-- end divider -->
```
