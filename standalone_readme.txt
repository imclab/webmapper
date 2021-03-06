WebMapper 0.2
GUI for libmapper OSC network
Stephen Sinclair, Aaron Krajeski & Jon Wilansky
Email: (aaron dot krajeski at mail dot mcgill dot ca)
http://libmapper.org

Dependancies:

	- Google Chrome, there has also been some preliminary testing in Firefox.

To Run:

	- Double click on 'WebMapper.app'
	- If Google Chrome is installed on your computer, but is not currently running, the GUI will open automatically.
	- If this does not happen for whatever reason, manually navigate to <localhost:50000> in Google Chrome (or Firefox if you're feeling lucky).

List View Command Keys:

	- 'c' : connect/link selected signals/devices
	- 'delete' : delete selected connections/links
	- 'm' : mute selected connections
	- 'alt+tab' : move right one tab
	- 'alt+shift+tab' : move left one tab
	- 'cmd+a' : select all currently visible connections/links	

	You can also mute connections while they are being made (press 'm' while connecting)


Grid view Command keys:

	click on cell: set the cell as selected
	COMMAND click a cell: select multiple cells

	arrows: move selected cell
	SHIFT + arrows: move selected cell by 3

	space: toggle selected cell(s)
	c: connect selected cell(s)
	d: disconnect selected cell(s)

	CTRL +: zoom in on active grid
	CTRL -: zoom out on active grid
	CTRL 0: zoom-to-fit on active grid
	CTRL 1: switch to SPLIT view
	CTRL 2: switch to DEVICES only view
	CTRL 3: switch to SIGNALS only view

	ALT leftArrow: set DEVICES grid as active
	ALT rightArrow: set SIGNALS grid as active
	ALT up/down arrows: cycle through presets

Grid View Instructions: 

- There are 2 grids. The left side is the DEVICES grid, the right is the SIGNALS grid. 

- To view signals in the SIGNALS grid: select cells (or labels) on the DEVICES grid and press the "Add"/"Remove" button ('a'/'s' keyboard shortcut). This will include/exclude the selected devices in the SIGNALS grid. Vertical/horizontal lines indicate if the device is included. 

- You can use the keyboard arrows to move the selected cell around. All keyboard shortcuts affect the 'active' grid, indicated by the little square in the upper left corner of the grid.

- You can save the current view in the SIGNALS grid as a 'preset' using the "SaveNew" button on the top right hand side. Note that changes to the current preset will not be remembered unless you press the "Update" button.

- Note the keyboard shortcuts for changing the active grid, moving the selected cell, toggling cells, loading presets, � they enable you to use the interface much more efficiently.

 *Grid view was developed and tested on Google Chrome only.




Hive view Command keys:

	c: connect selected cell(s)
	d: disconnect selected cell(s)

	CTRL 1: switch to view mode 1 (adapted Hive plot)
	CTRL 2: switch to view mode 2 (Hive plot)

Hive View Instructions: 

- The hive plot is a method for visualizing networks. In this view, the upper half of the plot is designated for source devices, and the lower for destinations. In view mode 1, an adapted hive plot, each device is given its own axis. In view mode 2, a traditional hive plot, source/destination devices are grouped along a single axis. 

- Although designed mainly as an aid for visualization, this view also provides the basic functionality to configure connections. Mouse over a device or signal in the list on the left hand side (or in the plot) to highlight its connections. Select signals by clicking its name in the list (or its node in the plot). Once a source and destination signal is selected, you can create or remove the connection by clicking on the blue bar at the bottom (or by using the keyboard shortcuts). 

- Connections on specific devices can be shown or hidden from view using the checkboxes in the list next to the device names.




Saving and loading notes:

  As of now saving and loading work via a na�ve approach. In the list view (currently the only view tested for saving and loading) save files will only save data for the active tab. Loading will only load connections for signals in the active tab. Though device names are recorded in save files, they are not actually used by the GUI to load mappings (this is done to make save mappings more portable).


Notes:

	- Balloon plot is brand new and has not yet been thoroughly tested.

	Have fun! Do report any bugs.
