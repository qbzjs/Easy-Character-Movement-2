Easy Character Movement 2
-------------------------

VERSION 1.2.1

	Character Movement (v1.0.6):
	----------------------------

	- Added CharacterMovement State data. This is the data needed to sync across the network ensuring proper simulation continuity.

	- Added networking examples for Major Unity networking libraries like Photon Fusion, FishNet, Mirror, etc.
	  Both, the Photon Fusion and FishNet examples implement server authoritative movement with client side prediction and reconciliation.

	- Minor bug fixes.
	
	
	NOTE: The full ECM2 networking update (i.e: Character(s) based development) is still in develepoment as it requires additional data sync and further tests.



VERSION 1.2.0


	- Added a new ReadMe welcome screen.


	Character Movement:
	-------------------

	- Greatly improved the 'Collide and Slide' algorithm. This is capable of correctly detecting and resolving overlaps found during the movement loop.

	- Added Use Flat Top option, when enabled will treat head collisions as if the character is using a shape with a flat top.

	- Exposed moving platform info through the movingPlatform property.

	- Minor bug fixes and improvements.


	Character(s):
	-------------

	- Character Monobehaviour methods are now private, this is to enforce the use of 'On' methods (ie: OnAwake, etc) instead.

	- Added a missing Custom Simulation Character example.

	- Added OnArrived event to the AgentCharacter.
	


VERSION 1.1.7

	- Fixed a bug with CharacterMovement SetDimensions and SetHeight functions not updating Collider size in editor.



VERSION 1.1.6

	- Minor bug fixes.



VERSION 1.1.5
 
	* W A R N I N G !
 
	  Please remove the ECM2 folder from your unity project before importing a new package.
  
	- New Folders structure. This lets you import CharacterMovement package only or full Easy Character Movement 2 package.
 
	- Added Assembly Definitions for CharacterMovement and ECM2 packages.
	
	- Minor bug fixes.
 
	- Fixed. CharacterMovement.detectCollisions not re-enabling collider.
 
	- Fixed. A case where fast moving characters keep stuck on swimming movement mode when leaving a PhysicsVolume.



VERSION 1.1.3

	- Minor bug fixes.



VERSION 1.1.1

	Character:
	----------

	- Fixed a bug causing some flags not being applied on release build.


	Character Movement:
	-------------------

	- Updated HitLocation ids to be on par with Collisionflags.

	- Removed deltaTime propety, now its handled as optional parameter, if no used it defaults to Time.deltatime.

	- Move methods now returns CollisionFlags to be on par with Unity's Character Controller.

	- Added CharacterMovement component performance test.

	- Fixed some minor bugs.



VERSION 1.1.0

	* W A R N I N G !

	Starting with this version, ECM2 is now a fully kinematic character controller and as a such it present significative changes, so:

	PLEASE BACKUP BEFORE UPDATE!


  How to update ?
  ===============

  	- Its recomended to completeley remove the ECM2 folder from your unity project before import new package from store.

  	- Once removed, import the package from asset store as regular.

  	- Please refer to changes document for a detailed list of removed / deprecated files and data structures and its new counterparts.
  	


VERSION 1.0

	- Initial release.


DISCLAIMER & LEGAL INFORMATION

THIS CODE AND INFORMATION IS PROVIDED "AS IS" WITHOUT WARRANTY OF ANY 
KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND/OR FITNESS FOR A
PARTICULAR PURPOSE.

YOU MAY NOT REDISTRIBUTE THIS SOURCE CODE IN WHOLE OR IN PART
WITHOUT WRITTEN CONSENT FROM THE CONTENT AUTHOR OR COPYRIGHT HOLDER.