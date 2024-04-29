Common Configs
=====

.. _commonConfigs:

.. contents::
   :local:

Common Configs
-------------------

.. _generalSettingsConfig:

General Settings Config
~~~~~~~~~~~~

Config to quickly on/off optional features.

Where To Find
~~~~~~~~~~~~

	.. image:: /images/configs/common/GeneralSettingsOnScene.png
	
Config Example	
~~~~~~~~~~~~

	.. image:: /images/configs/common/GeneralSettingsConfig.png

Player Settings
^^^^^^^^^^^^^^^^^^^^^^
	
**Player agent type:**
	* **Player** : player will be spawned.
	* **Free fly camera** :	flying camera will be spawned.
	
| **Player support** : on/off systems related to the player.	

Common Car Settings
^^^^^^^^^^^^^^^^^^^^^^

| **Car visual damage system support** : on/off visual hit feature for traffic vehicles by bullets.	

Traffic Car Settings
^^^^^^^^^^^^^^^^^^^^^^

| **Has traffic** : on/off traffic vehicle in the city.	

**Traffic baking type:**  
	* **Editor subscene** : all traffic entities are converted at editor subscene time.
	* **Runtime** : all traffic entities are converted at runtime.

| **Change lane support** : on/off feature to change lanes for traffic.
| **Traffic public support** : on/off public traffic vehicle in the city.	
| **Antistuck support** : on/off :ref:`antistuck <trafficCarAntistuckConfig>` feature for traffic vehicles.	
| **Avoidance support** : on/off :ref:`avoidance <trafficAvoidance>` of the vehicles.	
| **Car hit collision reaction** : on/off traffic collision reaction to other traffic cars.
| **Wheel system support** : on/off simple wheel system for traffic vehicles.	

Other Settings
^^^^^^^^^^^^^^^^^^^^^^

**Physics simulation type:**
	* **No physics** : dots physics off.
	* **Unity physics** : `Unity` dots physics on.
	* **Havok physics** : `Havok` dots physics on (havok physical package is required).
	
| **Cull physics** : on/off culling of the physics of dynamic objects that are far from the player.
| **Cull static physics** :on/off culling of the physics of static objects that are far from the player.
| **Force legacy physics** : force enable `built-in physics <https://docs.unity3d.com/Manual/PhysicsOverview.html>`_ , otherwise `built-in physics <https://docs.unity3d.com/Manual/PhysicsOverview.html>`_ will be disabled.

.. _propsDamageOption:

| **Props damage system support** : on/off damage systems for :ref:`props <propsInfo>`.
| **Target FPS** : target fps of the device.
| **Hide UI** : on/off UI.
| **Show FPS** : on/off fps ui panel.

Sound Configs
-------------------	

.. _soundConfig:

Common Sound Config
~~~~~~~~~~~~

	.. image:: /images/configs/common/CommonSoundConfig.png
	
| **Has sounds** : on/off `DOTS` sound systems.
| **Random horns sound** : on/off horn :ref:`sound <soundData>` system for traffic.
