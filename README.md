# PRO-C180
 
 
 Open Google Maps.
● Click on the “Show Your Location” button.

● Give permission to “Know yourlocation”.

● Click on the “Show Your Location” button again.

● Find the “blue” dot pointing to your location.

● Right-click on the “blue” dot and click on the first row (having latitude and longitude). It will be copied automatically.

● Paste it sowhere for later use.
Note: Use values till 7 decimal places
at max
---------------------------------------
Now once we have the location coordinates (latitude and longitude),

we can place any entity in A-Frame using the gps-entity-place component.

We can provide the latitude and longitude as values to this component in the string format:

gps-entity-place="latitude:<your-latitude>; longitude: <your-longitude>"
------------------------------------------------

GPS is a Global Positioning System. \n


It’s a satellite navigation system, which means location or navigation data are collected using satellites. 24 satellites are orbiting around Earth that send data to GPS devices like mobile phones and cars. 

GPS is a powerful technology and it can be used for:

Location—Determining a position. For example, finding your current location or the location of a particular place.

 Navigation—Getting from one location to another.
 
 Tracking—Monitoring objects/personal movement like in high-security jobs
 
Mapping—Creating maps of the world.
-----------------------------------------------------------------------------


To understand how we can use the A-Frame AR.js components to create location-based AR content, we will start with a demo scene. At a particular location (latitude and longitude), we will show a ball model.


we are going to use two components in  to place the 3D model at a particular location. 
1. gps-entity-place: When this component is attached in  tag, it will assign a position (latitude and longitude) on the Earth to that entity.
In this component, we can provide the latitude and longitude as values to this component in the string format: gps-entity-place="latitude: ; longitude: ".
For now, we will take the values of latitude and longitude from Google Maps.

2. look-at: This component makes sure the entity always points to the camera. We can give the value of the look-at component as a gps-camera so that it always faces the camera.

At last, to enable location AR, we need to set  as a GPS camera. We can use the gps-camera component for this.
In this component, we can use two attributes: minDistance and positionMinAccuracy.
