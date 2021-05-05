Table Examples

Tables are a great way of storig data in a structured way.
To create a table we would use <table></table> to create the table
Next we would use <tr></tr> to create the number of rows we want for our table
Next inside of the <tr> we would use <th></th> to specify a table header.
    The headers can either go along the top of the table or can go along the side of the rows as shown in table 5 in the table.html doc.
Next to fill in that data inside the <tr> we would then use <td></td> to fill in the table data.

Col or Row Span
    Sometimes some of the data needs to span multiple rows or columns.
    If your header/data nees to span multiple rows, inside the <th> or <td> we would add rowspan="value", were value is the number of rows you want to span across.
    If your header/data nees to span multiple columns, inside the <th> or <td> we would add colspan="value", were value is the number of columns you want to span across.
    If the data calls for it, you can put rowspan and colspan on the same <th> or <td>

Give your Tables and Name.
    So viewers of your table will know what's happening, you can add a table Caption to explain what the table is for.
    To give your table a Caption after creating the <table> before your first <tr> add <caption></caption> and inside you can insert text to explain your table.