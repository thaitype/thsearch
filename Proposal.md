
# Tokenizer

## Substring Indexing (N-grams)

During indexing, create smaller substrings (n-grams) for each token.
For example, for the word "โปรแกรม", create:

- Bigrams (2-character substrings): "โปร", "รก", "แก", "รม"
- Trigrams (3-character substrings): "โปรแ", "รแก", "แกรม"
  
Add these substrings as tokens in the inverted index.
Index Example:

```json
{
  "โปร": [{ "fileId": "file1", "positions": [0] }],
  "โปรแ": [{ "fileId": "file1", "positions": [0] }],
  "แก": [{ "fileId": "file1", "positions": [1] }]
}
```