# wdc
Wikidata categories
===================
Simply download the .zip file and unzip it.

To generate RDF statements for a Wikidata category item simply type in the command line

php concepts.php <wikidata_item_id>

Example for London category:

php concepts.php Q7149656

The file source.php is the configuration of the wikimedia sites used for the script. You can custom it using the site codes avalaible from the Wikidata API (see: https://www.wikidata.org/w/api.php?action=help&modules=sitematrix)

The time it will take the script to execute will depend on the complexity of the category and the sites from which it will extract the hierarchical relationships.

The result will be saved in a file in Turtle format in the "data" folder. The file name will begin with the wikidata id item used.
