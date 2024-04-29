.. _trafficPreset:

Presets
=====

* Preset contain prefabs that are converted to entities.
* There are several :ref:`Entity type <entityType>`. 
* The preset for conversion is selected from the :ref:`Entity type <entityType>` in the :ref:`Traffic Settings <trafficCarSettings>`.

	.. warning::
		If the :ref:`Vehicle Collection <vehicleCollection>` does not contain the appropriate :ref:`Prefab ID <trafficId>`, the `Prefab` will be ignored in the preset.
	
How To Create
----------------
	
Presets can only be created by using the :ref:`Car Prefab Creator <carPrefabCreator>` tool (step №5).

Where To Find
----------------

You can find in the scene here:

	.. image:: /images/entities/trafficCar/preset/PresetHolderExample.png
	
Entity Conversion
----------------

Make sure, that `TrafficCarEntityPoolBakerRef` in the :ref:`subscene <subscene>` has the correct preset. Read more about :ref:`config editing <configEdit>`.

	.. image:: /images/entities/trafficCar/howTo/Step6.png

Examples
----------------
	
	.. image:: /images/entities/trafficCar/preset/PresetHolderExample3.png
	`Hybrid custom entity player preset example`
	
	.. image:: /images/entities/trafficCar/preset/PresetHolderExample2.png
	`Simple physics entity traffic preset example`
	
	.. note::
		`Pure entity simple physics` type and `Pure entity no physics` type has the same preset.