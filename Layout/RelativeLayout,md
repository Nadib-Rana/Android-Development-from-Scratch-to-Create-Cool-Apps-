

---

### **RelativeLayout in Android**

- **Purpose:** Allows you to position child views relative to each other or the parent container.
- **Key Feature:** Flexible positioning of views based on other views or the parent.

#### **Common Attributes:**
1. **layout_alignParentTop:** Aligns the view to the top of the parent.
   - Example:
     ```xml
     android:layout_alignParentTop="true"
     ```

2. **layout_alignParentBottom:** Aligns the view to the bottom of the parent.
   - Example:
     ```xml
     android:layout_alignParentBottom="true"
     ```

3. **layout_below:** Places a view below another view.
   - Example:
     ```xml
     android:layout_below="@id/anotherView"
     ```

4. **layout_toRightOf:** Positions a view to the right of another view.
   - Example:
     ```xml
     android:layout_toRightOf="@id/anotherView"
     ```

5. **layout_centerInParent:** Centers the view horizontally and vertically within the parent.
   - Example:
     ```xml
     android:layout_centerInParent="true"
     ```

6. **layout_centerHorizontal:** Centers the view horizontally within the parent.
   - Example:
     ```xml
     android:layout_centerHorizontal="true"
     ```

7. **layout_centerVertical:** Centers the view vertically within the parent.
   - Example:
     ```xml
     android:layout_centerVertical="true"
     ```

#### **Example (Positioning Relative to Parent):**

```xml
<RelativeLayout
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <TextView
        android:id="@+id/title"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Title"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="20dp" />

    <Button
        android:id="@+id/button1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Submit"
        android:layout_below="@id/title"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="20dp" />

</RelativeLayout>
```

#### **Example (Positioning Views Relative to Each Other):**

```xml
<RelativeLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content">

    <TextView
        android:id="@+id/label"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Name" />

    <EditText
        android:id="@+id/input"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/label"
        android:layout_marginLeft="10dp"
        android:hint="Enter Name" />

    <Button
        android:id="@+id/submit"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/input"
        android:layout_alignParentRight="true"
        android:text="Submit" />

</RelativeLayout>
```
- **label** is positioned normally.
- **input** is positioned to the right of **label**.
- **submit** button is placed below **input** and aligned to the right of the parent.

---

#### **Summary:**
- **RelativeLayout** allows views to be positioned relative to other views or the parent.
- Use `layout_below`, `layout_toRightOf`, etc., to define relationships between views.
- Flexible layout for complex UIs but often replaced by **ConstraintLayout** in modern apps for better performance.

---

