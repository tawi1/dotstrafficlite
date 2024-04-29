.. _playerConfig:

Player Configs
=====

.. contents::
   :local:

Player Car Settings
-------------------	

.. _playerHybridDotsConfig:

Hybrid DOTS
~~~~~~~~~~~~

Player vehicle physics handled by `DOTS` systems.

	.. image:: /images/configs/player/PlayerCarSettings.png
	
.. _playerHybridMonoConfig:

Hybrid Mono
~~~~~~~~~~~~

How To Use
^^^^^^^^^^^^^^^^^^^^^^^^^^^

How to create player car with custom `Monobehaviour physics` read :ref:`this <playerHybridMono>`.	
	
Settings
^^^^^^^^^^^^^^^^^^^^^^^^^^^

	.. image:: /images/configs/player/PlayerCarSettingsMono.png
	
| **Max cast distance** : the cast distance of the box cast.
| **Extents multiplier** : extents multiplier of the box cast.
| **Min penetration distance** : the min collision distance to the collider when the collision force is active.
| **Penetration impulse** : the force that pushes car when it is inside another object.
| **Collide static** : on/off collision with static DOTS physics objects.
| **Collision mask** : collision mask with DOTS physics objects.