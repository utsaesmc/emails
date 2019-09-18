# Marketing Cloud Template Setup

Please enjoy this reference for basic markdown when setting up ESMC marketing cloud email templates. 

### Glossary
__Global__ : Without scope. (AKA, Should be done on every content block email wide.) 

__UTSA Orange__ : `#F15A22`

## `Global` Block Settings 

There are two global settings that shoud be on all content blocks.

* Margins should be set for `40px` on the left and right.
* Padding should be `0px` all around.

As a general rule. 
* Margins should be set for `0px` on the top and bottom.


*Some content blocks may have differing margin settings on top or bottom, but this will depend on placement within email or specific elements.* 

## `Global` HTML Editor Settings 
### Template Table HTML
Every Block should be wrapped in this code

```html
<table style="padding:0; margin:0; width:100%;">
  <tr>
   <td align="left" bgcolor="#ffffff" style="padding: 0px 0px 0px 0px; color: #002a5c; font-family: Helvetica, Arial, sans-serif; font-size: 15px; line-height: 22px; font-weight: 400;">
     
     <p style="margin: 0;">YOUR CONTENT IN HERE!</p>
    
    </td>
  </tr>
</table>
``` 

In the HTML view you should only see one `<table>` tag. If there are multiple `<table>` elements remove them! 

### Examples
Code you might find in HTML view
```html
<table style="width:100%; margin:0; padding:0;">
 
  <tr>
   <td align="left" bgcolor="#ffffff">
    <table style="margin:0; padding:0;">
     
      <tr>
      </tr><tr>
       <td style="padding-left: 0px; color: #002a5c; font-family: Helvetica, Arial, sans-serif; font-size: 18px; line-height: 24px; font-weight: 400;">
        <p style="margin: 0;">
         Roadrunner Days events begin on Friday, August 23 and we want you to participate in as many events as possible. It is a ton of fun and great way to start the new academic year.</p></td></tr></table></td></tr></table>

```
Change the code so that it looks like this
```html
<table style="padding:0; margin:0; width:100%;">
  <tr>
   <td align="left" bgcolor="#ffffff" style="padding: 0px 0px 0px 0px; color: #002a5c; font-family: Helvetica, Arial, sans-serif; font-size: 15px; line-height: 22px; font-weight: 400;">
     
     <p style="margin: 0;">Roadrunner Days events begin on Friday, August 23 and we want you to participate in as many events as possible. It is a ton of fun and great way to start the new academic year.</p>
    
    </td>
  </tr>
</table>
```

Using the `Template Table HTML` from above I placed the original `<p>Content Here</p>` tag inside where it says `[YOUR HTML CONTENT GOES HERE]`




 

## Paragrah Blocks

#### Block Settings
Paragraph blocks should have a `padding-bottom: 12px` set in the block settings section. 

#### HTML Editor
* If you prefer doing blocks with multiple paragraphs within them you will have to use `in-line` styles. 
* You will also have to manually remove these styles on the last `<p>` element of the block.
  
##### Examples
```html
<p style="margin: 0; padding-bottom:12px; font-size:20px; font-weight:bold;">Dear %%First Name%%,</p>
<p style="margin: 0; padding-bottom:12px;">We wanted to remind you of the on-campus VA ...</p>
```



