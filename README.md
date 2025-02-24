# TAFSIL
**TAFSIL**: Taxonomy Adaptable Fine-grained Entity Recognition through Distant Supervision for Indian Languages

- **TAFSIL Framework**: Uses [Wikipedia](https://www.wikipedia.org/), [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page), and taxonomy-specific mappings for entity extraction.
- **Stage 1 (Removing Non-Entity Links)**: Filters Wikipedia hyperlinks against a master dictionary, discarding non-entity mentions to reduce false positives.
- **Stage 2 (Exact Match Linking)**: Identifies unlinked entity mentions in Wikipedia using a trie to reduce false negatives.
- **Stage 3 (Fuzzy Matching)**: Handles spelling variations and agglutination using an edit distance heuristic for additional entity detection.
- **Stage 4 (Sentence Filtering)**: Uses [POS tagging](https://github.com/stanfordnlp/stanza) to remove sentences where entities are misclassified or missing.
- [**TAFSIL Datasets**](https://drive.google.com/drive/folders/1dLJNMBs_L-Yd6SGbkK20eZlw0oxbUHYY?usp=sharing): Created FgER datasets using Wikidata and Wikipedia dumps from June 1, 2024, covering 24 datasets in six languages across four taxonomies.


## TAFSIL Dataset Statistics

| Taxonomy     | Language  | Sentences | Entities  | Tokens     |
|-------------|-----------|-----------|-----------|------------|
| **FIGER**   | Hindi     | 697,585   | 928,941   | 25,015,025 |
|             | Marathi   | 138,114   | 193,953   | 4,010,213  |
|             | Sanskrit  | 18,946    | 25,515    | 520,970    |
|             | Tamil     | 523,264   | 825,287   | 17,376,040 |
|             | Telugu    | 419,933   | 616,143   | 10,103,255 |
|             | Urdu      | 641,235   | 1,219,517 | 43,556,208 |
| **OntoNotes** | Hindi   | 699,557   | 1,177,512 | 32,234,646 |
|             | Marathi   | 138,535   | 194,317   | 4,021,660  |
|             | Sanskrit  | 19,201    | 25,459    | 520,836    |
|             | Tamil     | 522,768   | 796,498   | 16,817,316 |
|             | Telugu    | 420,700   | 608,041   | 9,982,017  |
|             | Urdu      | 646,713   | 1,197,187 | 42,869,948 |
| **HAnDS**   | Hindi     | 702,941   | 1,108,130 | 30,249,166 |
|             | Marathi   | 139,163   | 195,251   | 4,039,536  |
|             | Sanskrit  | 19,294    | 25,581    | 523,540    |
|             | Tamil     | 526,275   | 804,132   | 16,988,161 |
|             | Telugu    | 422,736   | 611,226   | 10,034,077 |
|             | Urdu      | 647,595   | 1,200,111 | 42,988,031 |
| **MultiCoNER2** | Hindi | 643,880   | 799,987   | 21,492,069 |
|             | Marathi   | 125,981   | 174,861   | 3,628,450  |
|             | Sanskrit  | 17,740    | 23,372    | 479,185    |
|             | Tamil     | 464,293   | 690,035   | 14,583,842 |
|             | Telugu    | 392,444   | 561,088   | 9,266,603  |
|             | Urdu      | 603,682   | 1,069,354 | 38,216,564 |

Google drive link to download the datasets can be found [here](https://drive.google.com/drive/folders/1dLJNMBs_L-Yd6SGbkK20eZlw0oxbUHYY?usp=sharing).
