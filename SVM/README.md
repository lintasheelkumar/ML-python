# Pokemon Classification

A PokeDex - a Pokemon Detector Device which classifies these Pokemons - Pokemons like Bulbasaur, Pikachu, and Charmender.
The code contains an algorithm that classifies these Pokemons using an SVM classifier.

About Dataset
There are two folders Test and Train.

Train:
The train folder consists of a folder named Images which contains the images of three types of pokemon and a csv file which maps the images in the image folder to the name of that pokemon, The csv contains the field ImageId which is nothing but unique name given to each image and other field is NameOfPokemon which gives the pokemon name associated with that image.

Test:
Test also contains an image folder on which your model will be tested on and also there is a test csv file which only contains the name or ImageId of the image and gives the order in which each image is to be labelled .