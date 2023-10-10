# RLC-Toloka dataset

Sentences from the [Russian Learner Corpus](http://web-corpora.net/RLC) (RLC) corrected by users of the [Toloka](https://toloka.ai) crowdsourcing platform

The dataset was created as part of a project supported by the [Faculty of Computer Science](https://cs.hse.ru/en/), [HSE University](https://www.hse.ru/en/).

The file `rlc-toloka.csv` contains corrections for 34150 sentences. Every sentence was corrected by several of 4866 users. Each of the 213683 lines of the dataset corresponds to a correction of a single sentence by a single user.

## Format
- **sentence_id:** The sentence ID, a number between 1 and 34303.
- **user_id:** The ID of the Toloka user who corrected the sentence, a number between 1 and 4866.
- **original_sentence:** The original sentence from RLC corresponding to `sentence_id`.
- **corrected_sentence:** The correction proposed by the user.
