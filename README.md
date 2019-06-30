# Typo-proof GE search

This is a small prototype to show how a typo-proof GE search could be implemented.
I extract the character birgrams and trigrams from all GE items
bigrams are all two consecutive characters in a string, trigrams the same but with three characters (can be extended to any n-gram). E.g: "bucket" -> bu uc ck ke et / buc uck cke ket

Then after entering a query, I extract the bigrams and trigrams from the query and count the overlap between the query and each item and sort the items based on this count. This can of course be extended to be much more accurate by taking into account complete matches, long item name penalty, etc.
