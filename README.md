# Random Ipsom
A latin text generator similar to Lorem Ipsum. The plugin outputs randomly ordered paragraph text with three variations. You can use a random word count, a specific word count or inject random text into an existing text block.

## Usage variations

### Random word count (default)
- Create a new text layer on the canvas
- Run the plugin, and it will generate random text with a random word count

**Example**

    Type something


### Specified word count
- Create a text layer, and replace the contents with :13 (this is a word count tokken)
- Run the plugin, this will generate thrteen random words.

**Example**

    :13

### Inject random content
- Edit an existing paragraph, and inset counter tokkens on their own line (e.g. :23)
- Run the plugin, this will replace each tokken with a coresponding random sentence.

**Example**

    This is a sentence. We don't want to change this.
    :8
    Then there is another sentence, that we want to keep as it is.
    :13
    The end.


## Things to note

There is a minimum word count, three, this comes from "Lorem ipsum dolor", there is no maximum word count. If you generate a random paragraph, and run the plugin again, it will respect the existing word count. The plugin will generate random content on a text block that are named "Type something", to prevent acciedents just rename the layer to something meaningful.
