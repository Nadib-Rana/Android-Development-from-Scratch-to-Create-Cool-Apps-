In Android, **layout attributes** such as `wrap_content`, `match_parent`, and `gravity` are essential for defining how views are displayed within a layout. Here's a simplified overview of each:

### 1. **wrap_content**
- **Definition**: The view will size itself to fit the content it contains. The dimensions of the view will expand only as much as needed to display the content.
- **Usage**: Commonly used for views like `TextView`, `Button`, etc., where you want the view to be just large enough to hold its content without any extra space.

#### **Example**:
```xml
<TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Hello, World!" />
```
In this example, the `TextView` will be only as wide and tall as necessary to display the text "Hello, World!".

### 2. **match_parent**
- **Definition**: The view will expand to fill the entire space available to it in the parent layout.
- **Usage**: Used when you want a view to take up as much space as possible within its parent container.

#### **Example**:
```xml
<Button
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:text="Click Me!" />
```
In this example, the `Button` will stretch across the entire width of its parent while only taking enough height to fit its text.

### 3. **gravity**
- **Definition**: Specifies how the content within a view should be aligned. It determines the position of child views or content inside a parent view.
- **Usage**: Commonly used in layouts like `LinearLayout`, `FrameLayout`, and views like `TextView` to control the alignment of the text or other views.

#### **Example**:
```xml
<LinearLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:gravity="center"> <!-- Centers child views horizontally and vertically -->
    
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Centered Text" />
</LinearLayout>
```
In this example, the `TextView` is centered within the `LinearLayout` because of the `gravity` attribute.

### **Summary of Terms**:
- **wrap_content**: View size adjusts to fit the content.
- **match_parent**: View expands to fill the available space in the parent layout.
- **gravity**: Controls the alignment of content within a view.

