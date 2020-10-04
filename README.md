# nasa_gw_as

# Abstract

We are trying to create a prediction model of gravitational waves and visualisation based on its characteristics to find wormholes, and also we are creating a live asteroid tracking with prediction model for impacting the earth.

# Goals
To increase the accuracy of prediction of gravitational waves and asteroid alert.
Try to achieve a live asteroid system where we can surface the names of asteroids that could collide with earth from the asteroid visualization model.
Identifying wormholes by finding similar gravitational energy signatures in different regions of space.

# Problem
We are aiming to solve two different problems:
1) Detecting and proving the existence of possible interstellar wormholes
2) Live tracking asteroids and predicting when they will hit earth

### Wormholes
Wormholes are solutions to the Einstein field equations for gravity that act as "tunnels," connecting points in space-time in such a way that the trip between the points through the wormhole could take much less time than the trip through normal space.
Wormholes are possible, according to Einstein's general theory of relativity, but nobody has ever spotted one. They are expected to require extreme gravitational conditions, such as those present at supermassive black holes like Sagittarius A* to form and are most likely to be found near one.

### Asteroid tracking
Asteroids are small rocky bodies that orbit the sun. They are mostly found in the asteroid belt between mars and jupiter. Occasionally, asteroids' orbital paths are influenced by the gravitational tug of planets, which cause their paths to alter. It is believed that most extinction events in the history of our planet have been caused by asteroids colliding with earth. Hence, it is in our interest to detect, catalogue and track asteroids that may impact earth in the future.

# Solution

### Wormhole Identification
If a wormhole does exist at supermassive blackholes like Sagittarius A*, nearby stars would be influenced by the gravity of stars at the other end of the passage. One star should feel the gravitational influence of the star that’s on the other side due to the gravitational flux going through the wormhole. Each star has a unique gravitational energy signature, and if the gravitational energy signature of one star is detected at the other star, it probably means that there is a wormhole connecting them.

### Data
LIGO(Laser Interferometer Gravitational-wave Observatory) is the world's largest gravitational wave observatory. It collects information about gravitational waves from large gravitational events, and makes it available for anyone to use here.
We also used NASA’s data on Black Hole - Neutron Star Binary Mergers here
We used this to plot a q-transform of the data, which visually represents the frequency or energy of a gravitational source over time in a spectrogram. We then tag this as the unique gravitational energy signature of the source.If the same plot is seen elsewhere, it could indicate the presence of a wormhole in that area.

### Model Training
We have built, trained, evaluated and inspected a convolutional neural network on the above datasets. The CNN classifies spectrograms representing different types of glitches in gravitational waves into 22 classes like blip, koi - fish, chirp etc.
By classifying the data into similar classes, we can better identify identical or extremely similar gravitational energy signatures.
This classified data, along with the model, exposed as an API can help identify wormholes.

### Results
We have achieved an accuracy of 99.7% in classifying different types of gravitational waves. 
