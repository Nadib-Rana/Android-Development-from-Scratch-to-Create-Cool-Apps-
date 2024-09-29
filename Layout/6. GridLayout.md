
---

### **GridLayout in Android**

- **Purpose:** Arranges child views in a grid format, where views can span multiple rows and columns.
- **Key Feature:** Provides more flexibility compared to **TableLayout**, allowing for complex layouts.

#### **Attributes:**
1. **rowCount:** Specifies the number of rows in the grid.
   - Example:
     ```xml
     app:rowCount="3"
     ```

2. **columnCount:** Specifies the number of columns in the grid.
   - Example:
     ```xml
     app:columnCount="2"
     ```

3. **layout_row:** Specifies the row index for a child view.
   - Example:
     ```xml
     app:layout_row="0"
     ```

4. **layout_column:** Specifies the column index for a child view.
   - Example:
     ```xml
     app:layout_column="1"
     ```

5. **layout_rowSpan:** Specifies the number of rows a view should span.
   - Example:
     ```xml
     app:layout_rowSpan="2"
     ```

6. **layout_columnSpan:** Specifies the number of columns a view should span.
   - Example:
     ```xml
     app:layout_columnSpan="2"
     ```

#### **Example (Basic GridLayout):**

```xml
<GridLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    app:columnCount="2"
    app:rowCount="2">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Row 0, Col 0"
        app:layout_row="0"
        app:layout_column="0" />

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Row 0, Col 1"
        app:layout_row="0"
        app:layout_column="1" />

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Row 1, Col 0"
        app:layout_row="1"
        app:layout_column="0" />

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Row 1, Col 1"
        app:layout_row="1"
        app:layout_column="1" />

</GridLayout>
```

#### **Example (Using Span):**

```xml
<GridLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    app:columnCount="3"
    app:rowCount="2">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Item 1"
        app:layout_row="0"
        app:layout_column="0" />

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Item 2"
        app:layout_row="0"
        app:layout_column="1"
        app:layout_columnSpan="2" /> <!-- Spans two columns -->

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Item 3"
        app:layout_row="1"
        app:layout_column="0" />

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Item 4"
        app:layout_row="1"
        app:layout_column="1" />

</GridLayout>
```
- In this example, **Item 2** spans across two columns.

---

#### **Summary:**
- **GridLayout** provides a grid structure for organizing UI elements with flexibility for spanning rows and columns.
- Use **layout_row** and **layout_column** attributes to define the position of child views.
- Ideal for creating complex, grid-based layouts.

---
