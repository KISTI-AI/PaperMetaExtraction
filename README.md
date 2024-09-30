
# 논문 메타데이터 추출 데이터(Extraction data from paper metadata)

## Outline
- The data for extracting metadata from PDF domestic papers.
- The data contains information in layout box extracted from each PDF paper with labels corresponding to metadata field types.
- The information in each layout box are unique code, text, coordinates(x0, y0, x1, y1) of box, width of box, height of box and font size.
- The file named as “train.txt” was constructed through the fully automatic inspection process. It contains a total of 5,241,746 labeled layout boxes for 295,306 papers in 503 journals. It was used as train set.
- The file named as “valid.txt” was developed through the manual inspection process by several annotators. It contains a total of 155,629 labeled layout boxes for 9,895 papers in 503 journals.
- The file named as “test.txt” was built through the manual inspection process. It contains a total of 159,925 labeled layout boxes for 10,119 papers in 503 journals. It was used as test set.

## Data format(TXT)
- In the files, each layout box is separated by a newline. And each paper is separated by two newlines
- The data structure of each layout box is as follows :
  "Unique code"(\t)"Metadata label"(\t)"Text"(\t)"x0 value "(\s)"y0 value"(\s)"x1value"(\s)"y1value"(\s)"width value" (\s)"height value"(\s)"font size"
  
|No.|Metadata Fields|Label|
|--|--|--|
|1|Title(in Korean)|title_ko|
|2|Title(in English)|title_en|
|3|Author Name(in Korean)|author_name_ko|
|4|Author Name(in English)|author_name_en|
|5|Author Affiliation(in Korean)|ko_org|
|6|Author Affiliation(in English)|en_org|
|7|Abstract(in Korean)|abstract_ko|
|8|Abstract(in English)|abstract_en|
|9|Keywords(in Korean)|kwds_ko|
|10|Keywords(in English)|kwds_en|
|11|DOI|doi|
|12|Journal name|journal|
|13|Out of Boundary|O|

## Data statistics
|Data|File name|#Journal|#Paper|#Layout Box|
|--|--|--|--|--|
|Train set|train.txt|503|295,306|5,241,746 |
|Valid set|valid.txt|503|9,895|155,629|
|Test set|test.txt|503|10,119|159,925|


##  Data download
http://doi.org/10.23057/48

## License
CC BY-NC
<br>(Copyright Holder : Korea Institute of Science and Technology Information)

