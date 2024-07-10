# RLC-Crowd dataset

Sentences from the [Russian Learner Corpus](http://web-corpora.net/RLC) (RLC) corrected by users of the [Toloka](https://toloka.ai) crowdsourcing platform

The dataset was created as part of a project supported by the [Faculty of Computer Science](https://cs.hse.ru/en/), [HSE University](https://www.hse.ru/en/). We thank Georgii Kolesnikov for his help in creating the dataset.

The file `rlc-toloka.csv` contains corrections for 34150 sentences. Every sentence was corrected by several of 4866 users. Each of the 213683 lines of the dataset corresponds to a correction of a single sentence by a single user.

The file `rlc-toloka-test-counts.csv` contains 33 sentences offered to a large number of users; users who repeatedly failed to produce expected corrections for such sentences were disqualified from performing further tasks. For each correction, the number of users who suggested this correction is indicated.

## Format

`rlc-toloka.csv`
- **sentence_id:** The sentence ID, a number between 1 and 34303.
- **user_id:** The ID of the Toloka user who corrected the sentence, a number between 1 and 4866.
- **original_sentence:** The original sentence from RLC corresponding to `sentence_id`.
- **corrected_sentence:** The correction proposed by the user.

`rlc-toloka-test-counts.csv`
- **sentence_id:** The sentence ID, a number between 1 and 34303.
- **original_sentence:** The original sentence from RLC corresponding to `sentence_id`.
- **corrected_sentence:** A correction of this sentence.
- **count:** The number of users who proposed this correction.

## Reference
Daniil Kosakin, Sergei Obiedkov, Ivan Smirnov, Ekaterina Rakhilina, Anastasia Vyrenkova, and Ekaterina Zalivina. 2024. [Russian Learner Corpus: Towards Error-Cause Annotation for L2 Russian](https://aclanthology.org/2024.lrec-main.1241). In Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024), pages 14240–14258, Torino, Italia. ELRA and ICCL.
