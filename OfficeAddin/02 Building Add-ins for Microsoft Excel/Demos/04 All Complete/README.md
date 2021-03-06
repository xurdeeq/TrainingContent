# Office Add-ins: Building Office Add-ins for Excel

This demo is an aggregate of the other three demos in the module. It demonstrates working with worksheets, tables, charts, add-in commands, and the Dialog API from and Excel Add-in.

## Running the project

The finished solution is provided in this folder to simplify demonstrations. If you want to run a finished project, clone the repository, run **npm install** (from the solution folder directory), then **npm run start** and follow one of these methods to sideload and test the Office Add-in.

* Windows: [Sideload Office Add-ins on Windows](https://docs.microsoft.com/en-us/office/dev/add-ins/testing/create-a-network-shared-folder-catalog-for-task-pane-and-content-add-ins)
* Word Online: [Sideload Office Add-ins in Office Online](https://docs.microsoft.com/en-us/office/dev/add-ins/testing/sideload-office-add-ins-for-testing#sideload-an-office-add-in-on-office-online)
* iPad and Mac: [Sideload Office Add-ins on iPad and Mac](https://docs.microsoft.com/en-us/office/dev/add-ins/testing/sideload-an-office-add-in-on-ipad-and-mac)

## Demo steps

1. On the **Home** menu, select **Show Taskpane**.

1. In the taskpane, select **Create Table**.

1. Select the **Filter Table** and **Sort Table** buttons, in either order.

1. Select the **Create Chart** button. A chart is created and only the data from the rows that have been filtered are included. The labels on the data points across the bottom are in the sort order of the chart; that is, merchant names in reverse alphabetical order.

1. Select the **Freeze Header** button.

1. On the **Home** ribbon, select **Toggle Worksheet Protection**. Note that most of the controls on the ribbon are disabled (and visually grayed-out) as seen in screenshot below.

1. Select a cell as you would if you wanted to change its content. You get an error telling you that the worksheet is protected.

1. Select **Toggle Worksheet Protection** again, and the controls are re-enabled, and you can change cell values again.

1. Reload the task pane by closing it, and then on the **Home** menu, select **Show Taskpane** to reopen the add-in.

1. Select the **Open Dialog** button in the task pane.

1. While the dialog is open, drag it and resize it. Note that you can interact with the worksheet and press other buttons on the taskpane. But you cannot launch a second dialog from the same task pane page.

1. In the dialog, enter a name and select **OK**. The name appears on the task pane and the dialog closes.