 **LinearLayout** 

---

### **LinearLayout in Android**

- **Purpose:** Arranges child views in a single direction: either vertically or horizontally.
- **Key Attribute:** 
  - `android:orientation="vertical"` or `android:orientation="horizontal"`

- **Use Case:** Simple layouts where elements are aligned in one direction (either a column or a row).

#### **Attributes:**
1. **orientation:** 
   - Defines the direction of layout (vertical or horizontal).
   - Example: 
     ```xml
     android:orientation="vertical"
     ```

2. **gravity:** 
   - Aligns all child views in the layout.
   - Example: 
     ```xml
     android:gravity="center"
     ```

3. **layout_weight:** 
   - Divides space proportionally between child views.
   - Example: 
     ```xml
     android:layout_weight="1"
     ```

#### **Example (Vertical Layout):**

```xml
<LinearLayout
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:gravity="center">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello, World!" />

    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Click Me" />

</LinearLayout>
```

#### **Example (Horizontal Layout):**

```xml
<LinearLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:orientation="horizontal"
    android:gravity="center">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Label" />

    <EditText
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:hint="Enter Text" />

    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Submit" />
    
</LinearLayout>
```

#### **layout_weight Example:**
- Distributes space proportionally between elements.
  
```xml
<LinearLayout
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="horizontal">

    <Button
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:text="Button 1"
        android:layout_weight="1" />

    <Button
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:text="Button 2"
        android:layout_weight="2" />

</LinearLayout>
```
In this example, "Button 1" will take up 1 part of the available space, while "Button 2" will take 2 parts.

---

**Summary:**
- **Vertical LinearLayout:** Arranges views in a column.
- **Horizontal LinearLayout:** Arranges views in a row.
- **Use layout_weight:** To distribute space between child views efficiently.

---
