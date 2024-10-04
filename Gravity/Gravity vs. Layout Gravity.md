In Android development, **Gravity** is a property used to control the positioning of views or
content within a view. It is commonly used with `TextView`, `ImageView`, or `LinearLayout` to
specify how the content should be aligned within the boundaries of that view.

Here’s a breakdown:

1. **Gravity vs. Layout Gravity**:
   - **`android:gravity`**: Specifies how the content inside a view (e.g., text in a `TextView`) should be aligned.
   - **`android:layout_gravity`**: Specifies how the view itself should be aligned within its parent container.

### Common Gravity Values:
- `center`: Centers the content horizontally and vertically.
- `center_horizontal`: Centers the content horizontally.
- `center_vertical`: Centers the content vertically.
- `top`: Aligns the content to the top of the view.
- `bottom`: Aligns the content to the bottom of the view.
- `left`: Aligns the content to the left of the view (deprecated in RTL layouts).
- `right`: Aligns the content to the right of the view (deprecated in RTL layouts).
- `start`: Aligns content to the start (left in LTR and right in RTL layouts).
- `end`: Aligns content to the end (right in LTR and left in RTL layouts).

### Example Usage:

In XML:
```xml
<TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Hello World"
    android:gravity="center"
    android:layout_gravity="center"
/>
```

In Java/Kotlin:
```java
TextView textView = findViewById(R.id.textView);
textView.setGravity(Gravity.CENTER);
```

In this example, `android:gravity="center"` centers the text inside the `TextView`, while `android:layout_gravity="center"` centers the `TextView` itself inside its parent layout.

