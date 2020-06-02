# Flag-Classification
Program in Python that identifies flags (American, Russian, Japanese, Canadian) in the International Space Station

Plan: Find whether a photo contains a flag, and then classify photos based on what flag (by country) it contains.
Ultimately, we wanted a better grasp on the culture between different countries when it came to representing themselves through their country’s symbol.

Model:
CNN,
Epochs: 75,
Training data : All flags and random pictures,
Testing data: NASA ISS Photos

Model 1: Train a model to recognize flags in the photo.
Training data had two categories (Flags and Non-flags),
Flags folder contained photos of all the flags,
Non-flags folder contained any photos without a flag

Model II: Identify what type of flag is in the photo (using photos with previously  identified  flags).
Training data (American, Japanese, Russian, and Canadian flags),
200+ flag images per country,
Search through the new folder of images that contain flags and have our program decipher which flag is being represented

Learning outcome in terms of goal:
Model II predicts many Americans flags and predicts them fairly well possibly because Americans are most “prideful” or because our program trains on American flags best. Same for Russian flags,
Lots of images where flags of many countries are near each other,
Many astronauts seem to wear uniforms with multiple countries flags (indication of camaraderie?),
Variety of forms for flags (usually color scheme in varying forms on uniform)

Learning outcome in terms of code:
Training photos drastically change the results,
Need to keep every consideration in mind (ex. Ask why model predicts flag for certain non-flag images to troubleshoot)
