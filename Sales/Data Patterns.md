## Data Patterns

**Data Patterns** define numeric patterns for different types of barcodes for items, tenders, and so on.  

Data Patterns enable identification of any input accepted at a touch point, (e.g., a POS terminal, by scanning, swiping, or keying-in alpha-numeric characters) through any POS input peripheral (scanner, MSR) with a specific business entity, so that the entity related business process is activated automatically.  

The Emerald server supports recognizing data patterns either by the prefix length or by a regular expression (Regex).  

* **Prefix Length** - used to identify a data pattern by the prefix length. You can define a fixed prefix, or prefix length range. Once the Prefix length is defined, you can specify if the data pattern is decoded, encoded, or both.

    * Encoding - used to define Data Patterns in which the system encodes information into the data pattern, for example, a self-weigh barcode that is printed at the customer scale. The system encodes the item’s weight when placed on the scale into the barcode. The encoding process is responsible for generating the specific barcode following a request from a specific service.

    * Decoding - used to define Data Patterns from which information is extracted. For example, Item Price embedded Data Patterns. When an item barcode is scanned, the data such as the price, description, etc., can be identified. The Decoding process is responsible for identifying the relevant business entity and forward all extracted properties to it.

* **Regex** - Regular Expressions (Regex) is a sequence of characters that forms a search pattern. Data Patterns based on Regex are recognized by a wider set of rules based on Regex standards and are used for more complex scenarios.

A data pattern includes a predefined number of digits. Each set of digits is a field that includes data with specific information. There may be more than one data pattern with the same data pattern length and the same data pattern type.  

Each data pattern is set up with a validation code, identifier, and a set of fields that start in set positions within the data pattern. The recognizer of the data pattern can be a prefix and length but can also be a regular expression.  

Data patterns can be created with prefix ranges, and then linked to existing data patterns. For example, the Store Manager can specify that all item barcodes start with the prefix 22 and end with the prefix 23. You also have the option to group several data ranges into one pattern, avoiding multiple definitions.