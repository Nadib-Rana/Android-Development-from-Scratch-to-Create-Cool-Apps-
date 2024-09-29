### **What is a View?**
- A **View** is a basic UI element in Android that displays something on the screen and can respond to user actions.

### **Common Types of Views:**
1. **TextView**: Displays text.
   - Example: 
     ```xml
     <TextView android:text="Hello!" />
     ```

2. **EditText**: Allows user input of text.
   - Example:
     ```xml
     <EditText android:hint="Enter text" />
     ```

3. **Button**: A clickable button.
   - Example:
     ```xml
     <Button android:text="Click Me" />
     ```

4. **ImageView**: Displays an image.
   - Example:
     ```xml
     <ImageView android:src="@drawable/image" />
     ```

5. **CheckBox**: A box that can be checked or unchecked.
   - Example:
     ```xml
     <CheckBox android:text="Accept Terms" />
     ```

6. **RadioButton**: Selects one option from a group.
   - Example:
     ```xml
     <RadioButton android:text="Option 1" />
     ```

7. **ProgressBar**: Shows progress (loading, downloading, etc.).
   - Example:
     ```xml
     <ProgressBar style="?android:attr/progressBarStyleHorizontal" />
     ```

### **Key Points:**
- **Attributes**: Views have properties like width, height, and text.
- **Interactions**: Views can respond to clicks and touches.
- **Hierarchy**: Views can be nested inside other views to create layouts.

### **Example of Simple Layout:**

```xml
<LinearLayout android:orientation="vertical">
    <TextView android:text="Welcome!" />
    <Button android:text="Click Me" />
</LinearLayout>
```

### Summary
- Views are the building blocks of Android UIs, displaying content and allowing user interaction.
