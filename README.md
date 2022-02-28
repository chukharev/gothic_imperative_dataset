# gothic_imperative_dataset

## Synopsis 

The annotated dataset of verbs with the imperative meaning in Gothic.  

## How to read annotations

In `aspect_features.csv`, each row represents the annotations for a unique 
token.  At present, all verbs are second-person. 

### Field descriptions

The following are the descriptions of each field associated with a token: 
* `id`, a unique token identifier.
* `verse`, the verse of the Gothic bible in which the token appears 
  (abbreviated, so for example Matthew, Chapter 5, Verse 17 is written 
  `MATT 5.17`)
* `token`, the verbatim text of the token as it appears in the Gothic corpus. 
* `lemma`, the lemmatized token.  Lemmas are cited in the infinitive.
* `mood`, the grammatical mood of each token.  These are given as either
  `optative`, `imperative`, or `optative/imperative` (if ambiguous). 
* `number`, the number of the token.  Gothic distinguishes between 
  `singular`, `dual`, and `plural` numbers.

The remainder of the columns are features of semantic or lexical aspect.  Each
feature is associated with one of the following annotations:
* `TRUE`, if the feature applies to the token.
* `FALSE`, if the feature does not apply to the token.
* `NA`, if the applicability of the token is ambiguous. 

We encourage the reader to consult Maynard (2022) or Maynard et al. (2022) for
descriptions of the features.  
