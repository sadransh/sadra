---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Truveta Mapper: A Zero-shot Ontology Alignment Framework"
authors: [Mariyam Amir, Murchana Baruah, Mahsa Eslamialishah, Sina Ehsani, Alireza Bahramali, Sadra Naddaf-Sh, Saman Zarandioon]
date: 2023-09-02T02:12:50-07:00
doi: "https://arxiv.org/abs/2301.09767"

# Schedule page publish date (NOT publication's date).
publishDate: 2023-09-02T02:12:50-07:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "*The 18th International Workshop on Ontology Matching collocated with the 22nd International Semantic Web Conference ISWC-2023*"
publication_short: "ISWC-2023"

abstract: "In this paper, a new perspective is suggested for unsupervised Ontology Matching (OM) or Ontology Alignment (OA) by treating it as a translation task. Ontologies are represented as graphs, and the translation is performed from a node in the source ontology graph to a path in the target ontology graph. The proposed framework, Truveta Mapper (TM), leverages a multi-task sequence-to-sequence transformer model to perform alignment across multiple ontologies in a zero-shot, unified and end-to-end manner. Multi-tasking enables the model to implicitly learn the relationship between different ontologies via transfer-learning without requiring any explicit cross-ontology manually labeled data. This also enables the formulated framework to outperform existing solutions for both runtime latency and alignment quality. The model is pre-trained and fine-tuned only on publicly available text corpus and inner-ontologies data. The proposed solution outperforms state-of-the-art approaches, Edit-Similarity, LogMap, AML, BERTMap, and the recently presented new OM frameworks in Ontology Alignment Evaluation Initiative (OAEI22), offers log-linear complexity, and overall makes the OM task efficient and more straightforward without much post-processing involving mapping extension or mapping repair. We are open sourcing our solution."

# Summary. An optional shortened abstract.
summary: ""

tags: [NLP,deep learning, LLM, byT5]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://arxiv.org/abs/2301.09767
url_code: https://github.com/sadransh/ontology-matching-framework
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video:

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
