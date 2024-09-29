
### **Differences Between View and ViewGroup**

| Feature              | View                               | ViewGroup                          |
|----------------------|------------------------------------|------------------------------------|
| **Definition**       | A single UI element (like a button, text, image, etc.). | A container that can hold multiple child views (including other ViewGroups). |
| **Hierarchy**        | Cannot contain other views; it's a leaf node. | Can contain one or more child views and manage their layout. |
| **Purpose**          | Represents individual UI components. | Organizes and manages the layout of child views. |
| **Examples**         | `TextView`, `Button`, `ImageView`. | `LinearLayout`, `RelativeLayout`, `ConstraintLayout`. |
| **Layout Management**| Does not manage layout; it only draws itself. | Responsible for positioning and arranging its child views. |
| **Usage**            | Used for displaying content and user interaction. | Used to create complex UI layouts by grouping multiple views. |


