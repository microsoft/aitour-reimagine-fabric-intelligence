# React To Real-Time Events

I'm going to head back into the real-time hub, and we're going to jump into that third tab around Fabric events.
In this case, the Fabric events in the third tab provides that ability to listen to events, whether it's from Azure Blob Storage events or Fabric workspace item events so that I can actually listen to what's happening across my full organization.
Again, the examples of specific events that can happen are things like a specific items created or a new set of data is available, and it's really powerful and allows me to actually take those actions.
Selecting one of the options, I can see all the different event types that are available to me.
This helps me decide which ones I want to subscribe and listen to and take action.
Then once again, I have our set alert experience, and so I'm brought into that familiar experience where I can choose the events that I want to listen to.
In this case, I'm only going to listen to "FabricItemCreateSucceeded".
I can choose which workspace I want to monitor, and then I can directly set filters, so this lets me ensure that I'm only listening to events that include specific item name or an item kind that I want to listen to, if that's the scenario I'm going for, but the other option is just to listen to all of these event types within the specific workspace.
Once I've chosen the events, I'm going to go back into the pane.
Here you can see, again, I have the options of sending an e-mail or message me in Teams, but I can also run a Fabric item.
What this allows me to do is kick off my data pipeline or my notebook when this event comes in.
In this case, I'm going to trigger a "SalesPipeline", so whenever an item is created in that workspace, my SalesPipeline is automatically going to execute, so super powerful capabilities.

