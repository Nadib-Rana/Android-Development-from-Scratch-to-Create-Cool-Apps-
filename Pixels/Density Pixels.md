### **What are Density Pixels?**
- **Density Pixel (dp)**: A virtual pixel unit that helps ensure consistent sizing across devices with different screen densities.
- **Purpose**: dp is used to define layout dimensions and positions to maintain a uniform appearance on various screen types.

### **Why Use Density Pixels?**
- **Screen Density**: Different devices have different pixel densities, measured in dots per inch (dpi). For example, a device may have:
  - **ldpi**: Low density (120 dpi)
  - **mdpi**: Medium density (160 dpi) — baseline (1x)
  - **hdpi**: High density (240 dpi) (1.5x)
  - **xhdpi**: Extra high density (320 dpi) (2x)
  - **xxhdpi**: Extra extra high density (480 dpi) (3x)
  - **xxxhdpi**: Extra extra extra high density (640 dpi) (4x)

### **How It Works:**
- 1 dp is equivalent to 1 pixel on an mdpi screen (160 dpi).
- For higher density screens:
  - **hdpi**: 1 dp = 1.5 pixels
  - **xhdpi**: 1 dp = 2 pixels
  - **xxhdpi**: 1 dp = 3 pixels
  - **xxxhdpi**: 1 dp = 4 pixels

### **Example:**
- If you set a view's width to 100 dp:
  - On an **mdpi** screen, it will be 100 pixels wide.
  - On an **hdpi** screen, it will be 150 pixels wide (100 dp * 1.5).
  - On an **xhdpi** screen, it will be 200 pixels wide (100 dp * 2).

### **Usage in XML:**
```xml
<TextView
    android:layout_width="100dp"
    android:layout_height="wrap_content"
    android:text="Hello!" />
```

### Summary
- **Density pixels (dp)** are used in Android layouts to ensure that UI elements appear consistently across devices with varying screen densities, making it easier to create responsive and visually appealing applications.
