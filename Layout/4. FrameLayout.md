
---

### **FrameLayout in Android**

- **Purpose:** Used to stack views on top of each other, displaying one view at a time or layering multiple views.
- **Key Feature:** Displays the views in a stack, with the most recent one on top.

#### **Common Use Cases:**
- Overlaying views (e.g., adding a floating button over an image).
- Displaying one view at a time, such as using `ViewFlipper` for animations or transitions.

#### **Attributes:**
1. **layout_gravity:** Specifies how to align the view within the **FrameLayout**.
   - Example:
     ```xml
     android:layout_gravity="center"
     ```

#### **Example (Basic FrameLayout):**

```xml
<FrameLayout
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <ImageView
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:src="@drawable/sample_image"
        android:scaleType="centerCrop" />

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Overlay Text"
        android:textColor="#FFFFFF"
        android:background="#55000000"
        android:layout_gravity="center" />
    
</FrameLayout>
```
- **ImageView** takes the full screen.
- **TextView** is displayed over the image in the center with semi-transparent background.

#### **Example (Stacking Multiple Views):**

```xml
<FrameLayout
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <ImageView
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:src="@drawable/sample_image"
        android:scaleType="centerCrop" />

    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Floating Button"
        android:layout_gravity="bottom|end"
        android:layout_margin="16dp" />
    
</FrameLayout>
```
- **ImageView** fills the background.
- A **Button** is overlaid at the bottom-right corner, floating above the image.

#### **Example (Switching Between Views):**
- Only one view will be visible at a time.

```xml
<FrameLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content">

    <TextView
        android:id="@+id/view1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="View 1"
        android:visibility="visible" />

    <TextView
        android:id="@+id/view2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="View 2"
        android:visibility="gone" />
    
</FrameLayout>
```
- Initially, only **view1** will be visible, and **view2** will be hidden (`visibility="gone"`). You can toggle between the views programmatically.

---

#### **Summary:**
- **FrameLayout** stacks views, with the most recent added on top.
- Useful for overlaying or switching between views.
- Supports child view alignment using `layout_gravity`.

---
