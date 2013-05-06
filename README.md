Gravity Forms Inline Labels
==============

If you use Gravity Forms for Wordpress and your designer friends like inline-labels, this will be your friend. While you
will still have to style some small details, this will handle the basics of full width, two-field name fields, and the 
address block. This mixin was built after repeated head-banging caused by the forms at KVB60.org (e.g. [KVB Gala][1])

### Usage

This mixin assumes you have disabled Gravity Forms CSS. If you wish to not do so, you will need to inclde your rendered
CSS file after the Gravity Forms CSS file or edit the mixin to include !important tags.

To use the mixin, start with the list-item ID you wish to style, e.g. li#field_12_1, then call your mixin with the type of field 
you're adding.


* Default, full-width field: @include gf_field();
* First/Last Name Field: @include gf_field(name);
* Address Field (US Only, city/state/zip on one line): @include gf_field(address);
* Half-with fields floated left or right: @include gf_field(halfLeft) or @include gf_field(halfRight);

[1]: http://kvb60.org/gala/
