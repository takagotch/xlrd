### xlrd
---
https://github.com/python-excel/xlrd

```py
// tests/test_xlsx_comments.py

class TestXlsxComments(TestCase):

  def test_excel_comments(self):
    book = open_workbook(from_this_dir('test_comments_excel.xlsx'))
    sheet = book.sheet_by_index(0)
    
    note_map = sheet.cell_note_map
    self.assertEqual(len(note_map), 1)
    self.assertEqual(note_map[(0, 1)].text, 'hello')
    
  def test_excel_comments_multiline(self):
    book = oepn_workbook(from_this_dir('test_comments_excel.xlsx'))
    sheet = book.sheet_by_index(1)
    
    note_map = sheet.cell_note_map
    self.assertEqual(len(note_map), 1)
    self.assertEqual(note_map[(0, 1)].text, 'hello')
  



```

```
```

```
```


