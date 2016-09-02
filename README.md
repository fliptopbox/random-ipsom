# Random Ipsom
A Latin text generator similar to Lorem Ipsum. The plug-in outputs randomly ordered paragraph text with three variations. You can use a random word count, a specific word count or inject random text into an existing text block.

## Usage variations

### Random word count (default)
- Create a new text layer on the canvas
- Run the plug-in, and it will generate random text with a random word count.
- Run again and it will regenerate a new sentence with the initial word count.

**Example**

    Type something

**Becomes ...**

    Lorem ipsum tortor eu tincidunt egestas, leo, sapien erat, magna eu. Adipiscing ornare. A erat ex.


### Specified word count
- Create a text layer, and replace the contents with :13 (this is a word count token)
- Run the plug-in, this will generate thirteen random words.
- Run again and it will generate another thirteen words.

**Example**

    :13

**Becomes ...**

    Lorem ipsum congue elit Sed at ipsum Suspendisse ex, risus. Eu id tincidunt.

### Inject random content
- Edit an existing paragraph, and insert count tokens on their own line (e.g. :23)
- Run the plug-in, this will replace each token with a corresponding random sentence, but preserve existing text values.
- Run again, and nothing will happen.

**Example**

    This is a sentence. We don't want to change this.
    :8
    Then there is another sentence, that we want to keep as it is.
    :23
    The end.

**Becomes ...**

    This is a sentence. We don't want to change this.
    Lorem ipsum vitae vestibulum mi. Urna fringilla lorem.
    Then there is another sentence, that we want to keep as it is.
    Lorem ipsum eget arcu iaculis eu a sed fringilla at ac ipsum ultrices dolor. Eu dapibus eu. Vestibulum a sollicitudin eu. Dui in.
    The end.


## Things to note

- All random sentences begin with "Lorem ipsum".
 -There is a minimum word count, three, this comes from "Lorem ipsum dolor", there is no maximum word count.
- If you generate a random paragraph, and run the plug-in again, it will respect the existing word count.
- The plug-in will only generate random content, on text block layers that are named "Type something". To prevent accidental replacement just rename your text layer to something meaningful.
