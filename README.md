# Select-All-Row
This plugin about select all / select row.

#### Example structure select all
- [X] All
- [x] Row 1
- [X] Row 2
- [X] Row 3

#### Example structure select row
- [ ] All
- [X] Row 1
- [ ] Row 2
- [ ] Row 3

## Decription
  1. When where select All checkbox, automatically slave checkbox are getting selected.
  2. When where select all Row checkbox, automatically parent checkbox getting selected.

### Plugin Call
```
$('.select-all-slave').on('click', function(e){
  $(this).selectAll(e, 'select-slave', true); //(event, clicked element class, count flag) 
});
$('.select-slave').on('click', function(e){
  $(this).selectRow(e, 'select-all-slave', 'select-slave', true); //(event, parent class of clicked element, clicked element class, count flag)
});
```
