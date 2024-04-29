.. _packageInstallation:

Project Requirements
============

Minimum **Unity** version:
	* 2022.3.19+

**Required packages:**
	* `Entities 1.2.0 <https://docs.unity3d.com/Packages/com.unity.entities@1.2/manual/index.html>`_
	* `Entities.Graphics 1.2.0 <https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.2/manual/index.html>`_
	* `Unity.Physics 1.2.0 <https://docs.unity3d.com/Packages/com.unity.physics@1.2/manual/index.html>`_
	* `Custom Physics Authoring <https://docs.unity3d.com/Packages/com.unity.physics@1.2/manual/custom-samples-physics-components.html>`_
	* `Unity.Collections 2.4.0 <https://docs.unity3d.com/Packages/com.unity.collections@2.4/manual/index.html>`_
	* `Burst 1.8.12 <https://docs.unity3d.com/Packages/com.unity.burst@1.8/manual/index.html>`_ 

**Asset store packages:**
	* `Naughty attributes. <https://assetstore.unity.com/packages/tools/utilities/naughtyattributes-129996>`_
	* `Zenject. <https://assetstore.unity.com/packages/tools/utilities/extenject-dependency-injection-ioc-157735>`_
	* `FMOD <https://assetstore.unity.com/packages/tools/audio/fmod-for-unity-161631>`_ plugin for the sounds [optional].

Limitations
============

* The project overwrites the settings, so be sure to make a project backup before using the tool.
* :ref:`Roads <road>` can only be modified in the `Editor`.
* Vehicles with trailers or wagons are not currently supported for :ref:`NoPhysics <noPhysicsVehicle>`.

Package Installation
============

`Youtube tutorial. <https://youtu.be/q5S5cErl32g>`_

Steps
------------

#. Download & import from the `Unity Asset Store <https://u3d.as/2PCK>`_ .

#. First time initialization window will appear automatically or you can open it manually from the toolbar ``604Spirit/CityEditor/Window/Package Initialization``.

	.. image:: /images/gettingstarted/InitilizationWindow.png

#. Click `Load Packages` to start downloading the packages required for this tool.

	.. note::
		**Required custom packages:**
			* **Naughty Attributes** (`com.dbrizov.naughtyattributes`) - extension for unity inspector made by Denis Rizov, also you can manually download it from unity asset store `Naughty Attributes <https://assetstore.unity.com/packages/tools/utilities/naughtyattributes-129996>`_
			* **Extenject** (`com.svermeulen.extenject`) - library for injecting dependencies.

	.. note::
		**Script define symbols required for the project:**
			* **DOTS_CITY**
			* **UNITY_PHYSICS_CUSTOM**
			
	.. warning::
		* If you get the error 'No git executable was found', read :ref:`this <gitFix>`.
		* 'nunit.framework.dll' could not be found, read :ref:`this <nunitFix>`.
			
#. Restart the `Unity` project after all the packages have been downloaded.
			
#. Download the required assets from the `Asset Store`:

	.. note::
		**Required asset store packages:**
			* **FMOD** - asset store plugin for :ref:`game sounds <sound>` `FMOD <https://assetstore.unity.com/packages/tools/audio/fmod-for-unity-161631>`_
		
	.. note::
		**Script define symbols required for the project:**
			* **FMOD**
			
#. After that, press the `Add Scripting Define` button.
#. For more information on how to add sounds :ref:`click here <sound>`.
#. The next step is :ref:`to set up the new scene <cityCreation>` or launch the existing :ref:`Demo scene <demoOpening>`.