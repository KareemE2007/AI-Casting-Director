# Picking-the-Best-Cast-Using-Data-Science
The idea is to create an app containing a model that can look at (ideally at least a couple) books/comics/manga/video games or anything that’s not live action, take out the physical text from the work alongside resources from things like character wikis, and create a casting suggestion based on information about actors in Hollywood.

The first step involved looking at methods to compare strings computationally, and the best example found was in the OpenAI cookbook, specifically under the text embeddings folder.

There, the OpenAI embedding model (text-embedding-3-small), which vectorizes text (gives them a numerical magnitude and direction), was tokenized (for computing simplicity) then implemented among thousands of food reviews, showcasing its scalability for large datasets. The program shown in the example allowed the user to input any food, and the result showed the reviews that were most similar to the words inputted using a metric called cosine similarity, which, as the name implies, just computed the cosine of the angle between each vector that represents each word, and compares them as they range from -1 (least similar) to 1(most similar). 

This project involved implemented the same embedding model and similarity metric, but instead to match comic book heroes, specifically those in Marvel, to a large database of actors to see who matches the role best.

The standard we used was the Marvel Cinematic Universe, which is a good benchmark considering many fans were satisfied with the main cast, especially the outstanding Robert Downey Jr., who is considered the best casting choice in comic book movie history.

A tool that was useful to construct large datasets for actor descriptions was TMDB, which has many descriptions of actors that can be accessed through their API and from there manipulated

The method of data storage for this project is simple .json files, one for actor data that consists of names and descriptions, and another for marvel character data that contains names, traits and powers. 

Instead of processing thousands of marvel characters as we did actors however, the marvel character database is better done by hand, since nobody actually cares about Frog-Man (real Marvel character)


