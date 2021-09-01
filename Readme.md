<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/128654533/21.1.5%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/T329868)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->
<!-- default file list -->
*Files to look at*:

* **[MainWindow.xaml](./CS/NavBarExample/MainWindow.xaml) (VB: [MainWindow.xaml](./VB/NavBarExample/MainWindow.xaml))**
<!-- default file list end -->
# Building Outlook Navigation Menu Using OfficeNavigationBar and NavBarControl with TreeView


<p>In Outlook 2013, you may notice a special menu at the bottom for navigation between different views. You can build such a menu with DevExpress controls using <a href="https://documentation.devexpress.com/#WPF/clsDevExpressXpfNavigationOfficeNavigationBartopic">OfficeNavigationBar</a> and <a href="https://documentation.devexpress.com/#WPF/clsDevExpressXpfNavBarNavBarControltopic">NavBarControl</a>. OfficeNavigationBar takes all groups from NavBarControl and displays them in one line. To bind OfficeNavigationBar to NavBarControl, use the <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfNavigationOfficeNavigationBar_NavigationClienttopic">OfficeNavigationBar.NavigationClient</a> property. Please note that to display OfficeNavigationBar, it's necessary to set NavBarControl.Compact to false.</p>
<p>OfficeNavigationBar supports Peek Forms (popups displayed when you hover over an item). </p>
<img src="https://raw.githubusercontent.com/DevExpress-Examples/building-outlook-navigation-menu-using-officenavigationbar-and-navbarcontrol-with-treeview-t329868/15.1.4+/media/72ee6761-afad-11e5-80bf-00155d62480c.png"><br>
<p>To enable them, set <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfNavigationOfficeNavigationBar_ShowPeekFormOnItemHovertopic">ShowPeekFormOnItemHover</a> to true and specify the <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfNavBarNavBarGroup_PeekFormTemplatetopic">PeekFormTemplate</a> property.<br><br>Note that to display custom content in NavBarGroups, it's necessary to set <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfNavBarNavBarGroup_DisplaySourcetopic">NavBarGroup.DisplaySource</a> to "Content". It also makes sense to disable built-in group scrolling so that TreeView can use its own scrolling mechanism. To accomplish this task, set <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfNavBarNavBarGroup_GroupScrollModetopic">GroupScrollMode</a> to "None".</p>

<br/>


