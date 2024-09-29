
---

### **TableLayout in Android**

- **Purpose:** Arranges child views in a grid-like format with rows and columns, similar to an HTML table.
- **Key Feature:** Provides a structured way to display tabular data.

#### **Attributes:**
1. **stretchColumns:** Specifies which columns should stretch to fill extra space.
   - Example:
     ```xml
     android:stretchColumns="1"
     ```

2. **shrinkColumns:** Specifies which columns should shrink to fit content.
   - Example:
     ```xml
     android:shrinkColumns="0"
     ```

3. **layout_span:** Specifies that a view should span multiple columns.
   - Example:
     ```xml
     android:layout_span="2"
     ```

#### **Basic Structure:**
- A **TableLayout** contains one or more **TableRow** elements.
- Each **TableRow** can contain multiple child views.

#### **Example (Basic TableLayout):**

```xml
<TableLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:stretchColumns="1">

    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Header 1" />
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Header 2" />
    </TableRow>

    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Row 1, Col 1" />
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Row 1, Col 2" />
    </TableRow>

    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Row 2, Col 1" />
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Row 2, Col 2" />
    </TableRow>

</TableLayout>
```

#### **Example (Using layout_span):**

```xml
<TableLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content">

    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Merged Header"
            android:layout_span="2" />
    </TableRow>

    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Row 1, Col 1" />
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Row 1, Col 2" />
    </TableRow>

    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Row 2, Col 1" />
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Row 2, Col 2" />
    </TableRow>

</TableLayout>
```
- In this example, the first row has a header that spans across both columns.

---

#### **Summary:**
- **TableLayout** provides a way to organize UI elements in rows and columns, resembling a table structure.
- Use **TableRow** for each row and specify child views within it.
- Supports features like spanning multiple columns and stretching/shrinking columns.

---
!
