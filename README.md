# Responsive Layout with Navigation Bar and Cards Hover Effects

This responsive layout project has a NAVIGATION BAR that can be adapted to the screen and contents shown on CARDS with 
Hover Effects.

#### The Web Page can be found [HERE](https://willygoncalves2000.github.io/responsive-layout-with-navbar-and-cards/)!



### Deployment
To build the Responsive Layout, the checkbox was used:
```
   <input type="checkbox" id="check">
   <label for="check" class="checkbtn">
        <i class="fas fa-bars"></i>
   </label>
```
**Observation**: The class "fas fa-bars" refer to a icon available by the library Font Awesome. To use this library it is necessary
add the following tag: 
```
   <script src="https://kit.fontawesome.com/1dbca84bfc.js"></script>
```
The **_label_** is relationship with the **_input checkbox_** trought the *for* attribute.

The **_i_** tag was used to place the icon from the menu that work as a **_button_** when the device screen is small. While the screen **_width_**
is greater than **_915px_**, the Navigation Bar menu will have a horizontally positioned list in the upper right corner.
In this case, the **_input checkbox_** and the **_label_** stay oculte trough the value **none** in the **display** property:
```
.checkbtn{
    font-size: 30px;
    color: white;
    float: right;
    margin-top: 24px;
    margin-right: 40px;
    cursor: pointer;
    display: none;
}
#check{
    display: none;
}
```
When the screen has a **_width_** less than or equal to **_915px_**, the value of this property is changed to **block** in the **_label_**:
```
@media (max-width: 915px){
  .checkbtn{
    display: block;
  }
}
```
This causes the icon to appear on the screen, so list will give rise to this icon which, when clicked, 
will open a horizontal menu. 



