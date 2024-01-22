# indoler

This repository contains the dataset used in our undergraduate thesis. The dataset contains 993 annotated court decission document. The document was taken from [Decision of the Supreme Court of Indonesia](https://decision3.mahkamahagung.go.id/). the documents have also been tokenized and cleaned. The data is stored using JSONL format with fields as follows:

```json
{
	"id": "the internal id of the document",
	"owner": "the person who annotate the document",
	"lawyer": "whether the defendant has a lawyer present",
	"verdict": "The type of verdict given in the document (guilty, bebas, or lepas)",
	"indictment": "The type of indictment presented to the court (Tunggal, subsider, komul, alternatif, kombinasi, or gabungan)",
	"text": "Word-splitted text",
	"text-tags": "IOB formatted label"
}
```

## Here's two data from the dataset:

```json
[
	{
		"id": 2743,
		"owner": "agree",
		"lawyer": False,
		"verdict": "guilty",
		"indictment": "subsider",
		"text-tags": ["O", "O", "B-Nomor Putusan", "I-Nomor Putusan", "O", "O", "O", "O", "O", "O", "O", "B-Nama Pengadilan", "I-Nama Pengadilan", "I-Nama Pengadilan", ...],
		"text": ["\ufeffputusan", "nomor", "325/pid.b/2015/pn", "bwi", "demi", "keadilan", "berdasarkan", "ketuhanan", "yang", "maha", "esa", "pengadilan", "negeri", "banyuwangi", ...]
	},
	{
		"id": 2744,
		"owner": "agree",
		"lawyer": False,
		"verdict": "guilty",
		"indictment": "alternatif",
		"text-tags": ["O", "O", "B-Nomor Putusan", "I-Nomor Putusan", "O", "O", "O", "O", "O", "O", "O", "B-Nama Pengadilan", "I-Nama Pengadilan", "I-Nama Pengadilan", ...],
		"text": ["\ufeffputusan", "nomor", "285/pid.b/2016/pn", "sda", "demi", "keadilan", "berdasarkan", "ketuhanan", "yang", "maha", "esa", "pengadilan", "negeri", "sidoarjo", ...]
	}
]
```

We also provide the data we used in each split in CSV format.


## Contact
**evi.y [at] cs.ui.ac.id**. naradhipabhary27 [at] gmail.com
