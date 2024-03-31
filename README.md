# IR-Project: Wikipedia Search Engine 
Implementation Description:
Indexes and Data structures:
DL (Document Length): This dictionary holds the length of each document, enabling the 
search engine to swiftly access a document's length without scanning the entire content.
DT (Document Title): This dictionary records the title of each document, enhancing the 
presentation of search results for users.
Alongside the indexes for title, body and anchor, these data structures are in the bucket
provided above.

• Experimented with tf-idf algorithm and anchor text index for search engine 
on English Wikipedia corpus.
• Introduced BM25 algorithm which significantly improved Mean Average 
Precision at 40 (MAP@40).

• Utilized precalculated data structures (DL and DT) to speed up calculations.
• Implemented multithreading for sub-search functions to increase retrieval 
efficiency. Eventually it turns out that in Python Threading does not really 
have an advantage.

• Anchor index enhances search engine performance.
• BM25 is a superior alternative to tf-idf for ranking documents.
• Threading did not effect the performance.
