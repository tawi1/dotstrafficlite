.. _trafficArea:

Traffic Area
=====

`Traffic Area` is used for restricted traffic areas with an order of entry and exit.

Use-case examples: 
	* To enter a petrol station. 
	* Used for :ref:`large parking areas <roadSegmentCreatorParkingBuilder>`.

`Youtube tutorial. <https://youtu.be/KnLjpAt_AFE>`_

How To Create
------------

#. Create an empty `GameObject` and add :ref:`TrafficAreaAuthoring <trafficAreaSettings>` component
#. Set the :ref:`Button select type <trafficAreaSceneVisual>` to `Select node` value.
#. Enable the :ref:`Show scene nodes <trafficAreaSceneVisual>` option to see the :ref:`traffic nodes <trafficNode>` in the scene.
#. Set :ref:`New node type <trafficAreaSceneVisual>` to `Default` value.
#. Select `Default` nodes in the scene.

	.. image:: /images/road/trafficArea/TrafficAreaExample2.png
	`Selected Default nodes example`.
	
#. In the same way, select the `Queue` node in the scene.

	.. image:: /images/road/trafficArea/TrafficAreaExample5.png
	`Selected Queue node example`.
	
#. Select `Enter` node in the scene.

	.. image:: /images/road/trafficArea/TrafficAreaExample4.png
	`Selected Enter node example`.

#. Select `Exit` node in the scene.

	.. image:: /images/road/trafficArea/TrafficAreaExample6.png
	`Selected Exit node example`.
	
#. Adjust the :ref:`Max queue count <trafficAreaSettings>` depending on how many cars can fit in the queue without blocking other cars.
	
	.. image:: /images/road/trafficArea/TrafficAreaExample7.png
	`TrafficArea result example (parking created by` :ref:`ParkingBuilder <roadSegmentCreatorParkingBuilder>` `).`

.. _trafficAreaSettings:

Settings
------------

	.. image:: /images/road/TrafficArea.png
	
Settings
~~~~~~~~~~~~ 
	
| **Max queue count** : maximum number of cars in a queue (if the maximum number is exceeded the entrance node will be closed).
| **Max skip enter order count** : number of vehicles that can be let in at the entrance (1 value example: 1 enters vehicle - 1 exits - 1 enters - 1 exits).
| **Has exit order** : cars leave the `TrafficArea` on a queue basis.

.. _trafficAreaSceneVisual:

Scene visual
~~~~~~~~~~~~ 

| **Draw connection** : on/off visual connections.
| **Draw connection lines** : on/off connection lines to the :ref:`traffic nodes <trafficNode>`.
**Button select type:**
	* **Disabled**
	* **Remove node** : selected node will be removed from `TrafficArea`.
	* **Select node** : selected node will be added to `TrafficArea` with the select `New node type`.
| **Show traffic area node type** : :ref:`nodes <trafficNode>` with the selected :ref:`node type <trafficAreaNodeType>` will be displayed in the scene.
| **Show scene nodes** : on/off display add buttons paths to `TrafficArea`.
| **New node type** : :ref:`TrafficNode <trafficNode>` with the selected :ref:`node type <trafficAreaNodeType>` will be added to the `TrafficArea`.

.. _trafficAreaNodeType:

Node type
~~~~~~~~~~~~ 

* **Default** : a node which is included in the `TrafficArea` but does not belong to one of the types listed below.
* **Enter** : entrance node to the `TrafficArea` (if the maximum number of vehicles in the queue is exceeded, the node will be closed).
* **Queue** : node in front of which a line of cars is waiting.
* **Exit** : when it passes this node, the car leaves the `TrafficArea`.