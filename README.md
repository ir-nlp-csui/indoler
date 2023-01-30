# indoler

This data set consists of Indonesian court decision documents that have been annotated as legal entities. There are 1010 decision documents on the website [Decision of the Supreme Court of Indonesia](https://decision3.mahkamahagung.go.id/). Available documents have been tokenized and stored using json format. Detailed dataset information is as follows:

```json
{
	"doc" : "document number",
	"sentence" : "sentence number",
	"words" : "array of words in sentence"
	"labels" : "Tagging of words"
}
```

## Here's one sentence from the dataset:

```json
{
	"doc": "doc: 1",
	"sentence": "seq: 1",
	"words": ["PUTUSAN", ".", "NOMOR", ":", "1974", "/", "Pid", ".", "Sus", "/", "2012", "/", "PN", ".", "JKT", ".", "BAR", ".", "DEMI", "KEADILAN", "BERDASARKAN", "KETUHANAN", "YANG", "MAHA", "ESA", "."],
	"labels": ["O", "O", "O", "O", "B_putusan", "I_putusan", "I_putusan", "I_putusan", "I_putusan", "I_putusan", "I_putusan", "I_putusan", "I_putusan", "I_putusan", "I_putusan", "I_putusan", "I_putusan", "I_putusan", "O", "O", "O", "O", "O", "O", "O", "O"]
}
```

## Reference
Please cite the following paper if you use this dataset:

**Nuranti, E. Q., and Yulianti, E.,** <a href="https://ieeexplore.ieee.org/abstract/document/9263157">“Legal Entity Recognition in Indonesian Court Decision Documents Using Bi-LSTM and CRF 597 Approaches,”</a> 2020 International Conference on Advanced Computer Science and Information Systems (ICACSIS), pp. 429–434.

## Contact
**evi.y [at] cs.ui.ac.id**
