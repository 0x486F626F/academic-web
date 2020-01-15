---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Carousel: Low-Latency Transaction Processing for Globally-Distributed Data"
authors: [Xinan Yan, Linguan Yang, Hongbo Zhang, Xiayue Charles Lin, Bernard Wong, Kenneth Salem, Tim Brecht]
date: 2020-01-14T18:23:29-05:00
doi: "https://doi.org/10.1145/3183713.3196912"

# Schedule page publish date (NOT publication's date).
publishDate: 2020-01-14T18:23:29-05:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "Carousel"
publication_short: "carousel"

abstract: "The trend towards global applications and services has created an increasing demand for transaction processing on globally-distributed data. Many database systems, such as Spanner and CockroachDB, support distributed transactions but require a large number of wide-area network roundtrips to commit each transaction and ensure the transaction’s state is durably replicated across multiple datacenters. This can significantly increase transaction completion time, resulting in developers replacing database-level transactions with their own error-prone application-level solutions. This paper introduces Carousel, a distributed database system that provides low-latency transaction processing for multi-partition globally-distributed transactions. Carousel shortens transaction processing time by reducing the number of sequential wide-area network round trips required to commit a transaction and replicate its results while maintaining serializability. This is possible in part by using information about a transaction’s potential write set to enable transaction processing, including any necessary remote read operations, to overlap with 2PC and state replication. Carousel further reduces transaction completion time by introducing a consensus protocol that can perform state replication in parallel with 2PC. For a multi-partition 2-round Fixed-set Interactive (2FI) transaction, Carousel requires at most two wide-area network roundtrips to commit the transaction when there are no failures, and only one round trip in the common case if local replicas are available."

# Summary. An optional shortened abstract.
summary: ""

tags: []
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: "files/carousel-sigmod-2018.pdf"
url_code:
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video: "https://www.youtube.com/watch?v=TiAcfrBuYyk"

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
