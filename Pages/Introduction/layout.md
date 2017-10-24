# Layouts

Use structural templates to design pages and create consistency across the product.

// todo: add mockup to demonstrate

### Basic Layout

**Sidebar **

* Global navigation 

**Top bar**

* Breadcrumb 
* Utility links on the top right \(e.g., help and user menu\)

**Main area**

* Title
* Content 

### Table Layout

**When to use**

* Display a list of structured data in the main area

**Interaction**

* Main actions\(create\), Filter, Sections, Sort, Pagination

**Example**

* Cluster list page, Job list page

### Form Layout

**When to use**

* Display a form in the main area. 

**Interaction**

* Buttons on the top \(close to the title\), or on the bottom
* Progressive disclosure, e.g., create a new table 

**Example**

* Create new cluster, Create new library.

### Detail Page Layout

**When to use**

* Every entity \(cluster, table, job, job run, library\) in the product has a detail page to display information and provide actions.
* Group related content and prioritize those based on the use case.

**Example**

* Notebook: title, context bar \(menu, toolbar\), widget bar \(toggle between visible and hidden\), cells, right panel \(toggle between visible and hidden\)
* Table: title, action buttons, section titles, tables
* Job: title, action buttons, meta data, section titles, tables 
* Cluster: title, action buttons, tab, form \| table \| meta data + table 
* Library: title, action buttons, meta data, table 

### **Responsive UI **

* Breakpoints: 960, 1280, 1440, 1600 
  * for layout under 960px wide, set min width for components    
  * for layout over 1600px wide
    * continue to grow for table and notebook cell \(expand\)
    * for fixed elements or elements with a max width, remain left aligned while the right margin grows
* 12 column grid layout with gutter \(24px\) 
* Panel influence on the grid
  * We have 2 different panels in the product: file browser and the notebook right panel
  * Currently file browser panel pushes the main content to the right. It squeezes some content \(notebook, table\), but push others off screen \(home view\)
  * Notebook right panels: revision history and comments squeeze the cells while schedule and dashboard property overlay. 

### References:

[https://material.io/guidelines/layout/responsive-ui.html](https://material.io/guidelines/layout/responsive-ui.html)

