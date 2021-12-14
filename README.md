
# PyNFT

## One Stop tool for NFT generation

---

* ### Use Case

  * Generation of any number of images from base images, as required by NFT Projects
  * Currently only supports 2D .png's and OpenSea metadata standards

* ### Requirements

  * Python 3 or later
  * Pillow

  ```bash
  python3 -m pip install --upgrade pip
  python3 -m pip install --upgrade Pillow
  ```

  * sys, os, random, json - included in a standard installation of Python

* ### Process

  * Step 1

    * Create your art and store it in one of the supported formats
    * __All individual file names must be unique__
    * __Make Sure there are no trailing spaces in the filenames and each of the filename only have one space between two words__
      * RedShirt.png is valid
      * Red Shirt.png is valid
      * Red  Shirt.png is not valid -- 2 spaces between 'Red' and 'Shirt'
      * Red Shirt .png is not valid -- Trailing space after 'Shirt'
    * Arrange your art files in the 'Assets'folder with the following file structure
      * Assets
        * Trait 1
          * Unique Name 1
          * Unique Name 2
          * Unique Name 3
          * . . .
        * Trait 2
          * Unique Name 8
          * Unique Name 9
          * Unique Name 10
          * . . .
        * . . .

  * Step 2
    * Run the "To be filled in" file and follow its steps
    * This will save your selections as 'data.json' and will be used in the subsequent steps this will include do rarity for other traits, metadata preferences and the order of layers in which the traits are to be pasted on top of each other
  * Step 3
    * Run the "To be filled in" file and follow it will generate a 'selection.json'.This will hold the selection for each and every NFT of your project
    * __DO NOT LOSE THIS AFTER YOU MINT__

  * Step 4
    * Run the "To be filled in" file and it will generate all the combined art and metadata for each NFT
    * Run the "To be filled in" file and it will sieve all of your output art and store in the 'Sample' folder only those you need to see manually. This is bit hard to explain in words but the implication is if there is any sort of clipping or overlap in the entire output art, it will also be present in the 'sample' folder also if the aren't any issue in the 'sample' folder then you can rest assured that the entire output doesn't have any issues either
    * On finding any sort of clipping or overlap of traits you can fix the base images in the 'Assets' folderand rerun the "To be filled in" file
