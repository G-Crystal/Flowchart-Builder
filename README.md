Flow Chart Builder Specification
--------------------------------


**Overview**


Our objective is to build a drag and drop flow chart builder using jsPlumb community edition and jQuery (see figure 1.0) with below capabilities:

 **1. A canvas area**
 This is where the flow chart is designed by dragging elements from the blocks(6) pane. The user can zoom in/ out and move around the canvas area.
 
 **2. Flowchart elements**
 These are flow chart elements making-up the workflow template. Users can connect elements using process flow connectors (lines). Elements can have multiple input ports and output ports depending on the element type. In a flowchart an element can not connect to itself using a process flow.
 
 **3. Pane slider/ explorer pane**
 Explorer pane has two vertically scrollable windows. Top one (4) for setting of an element selected on the canvas, and the bottom (6) for exploring element types available to build the workflow. When a user select an element on the canvas, explorer pane slides to the left to show the details. The user can click on the pane slider button to bring in and out the explorer.
 
 **4. Settings window**
 Provides the capability to update element properties.These properties depend on the the selected element type, and will include text fields, drop downs and date selectors, etc to update the properties. Setting window will allow vertical scrolling for the overflow.
 
 **5. Height Adjuster**
 Allows the user to slide up or down increasing or decreasing the window heights of settings or blocks windows.
 
 **6. Elements/ Blocks window**
 Provides a listing of available element types to build the flowchart, along with a description.

The user can click/drag to add an element to the canvas.
This area is vertically scrollable.

**Type of elements**

 **1. Question**
 Has a label
Has only one input port and two output ports (yes and no)

 **2. Action**
 Has a label
User can select from a list of available automatic actions
Has multiple input ports
User can select whether just one input should trigger the action, or whether all inputs are required to trigger the action

 **3. Connector (used to indicate an integration)**
 Has a label
User can provide an endpoint url
user can provide username, password or user can provide API key
user can define the response type (boolean, data string, number, text)


**Exporting and Importing**

 - The flow chart builder should provide the capability to export the
   flowchart definition into JSON format.
   
 -  The flow chart builder should be able to load a JSON file and draw
   the chart on the canvas.
 
 
**Planned Iterations**
- Iteration 01 
		- Create page structure. 
		- Set-up jsPlumb canvas Implement
		- the capability for the user to drag an action element from the
		- explorer to the canvas. Implement the capability for the user to
		- connect multiple action elements on the canvas Implement the
	   -  capability to export the flowchart into JSON.

**Resources**

Flow Chart builder demo: https://jsplumbtoolkit.com/demos/toolkit/flowchart-builder/index.html


jsPlumb Documentation: https://jsplumbtoolkit.com/community/doc/home.html




 
 
![enter image description here](https://drive.google.com/file/d/0B5PrAhvbNvJfdTZ4eFdiUmVRbVU/view?usp=sharing)


Figure 1.0
