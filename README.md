Copyright 2021 by Southeast University & Nanjing University of Posts and Telecommunications. 

Time: 13/11/2021  Authors:  Heng Zhou & Weizhuo Li & Buye Zhang 

Mail: zhouheng2020@seu.edu.cn & liweizhuo@amss.ac.cn & zhangbuye@seu.edu.cn

Description: [MAKG](http://www.makg.com.cn/) is a mobile applications knowledge graph. You can use its original resources and visit the [website](http://www.makg.com.cn/) to enjoy its services.

## 1. Introduction：
In this project, we present a mobile application knowledge graph, namely MAKG, which aims to collect the apps from various resources (e.g., application markets, encyclopedias, news). 

We design a lightweight ontology of apps. It can bring a well-defined schema of collected apps so that these apps could share more linkage with each other. Moreover, we employ the algorithms of information extraction and knowledge alignment during the process of construction so as to enhance structured triples to MAKG. Finally, we list several use-cases about MAKG that are helpful to provide better services for security analysts and users.


## 2. Usage:
MAKG consists of five important resources, including Ontology (Knowledge Schema), AppMarket-Triples, Encyclopedias, AppMarket-Alignments, Extraction-Triples.

A technical report with details of these resources and related evaluations can be downloaded in the same address.

### Ontology:
We design one lightweight ontology of apps. It can bring a well-defined schema of collected apps so that these apps could share more linkage with each other.
It contains 26 basic classes, 11 relations and 45 properties. 

We provide two files (appOntology.owl and appSchema.xlsx) for researchers to use it. For the former file, it needs to install [protege](https://protege.stanford.edu/) to open it.


### AppMarket-Triples:
This dataset contains raw triples crawlled from [Huawei App Market](https://appgallery.huawei.com/), [Xiaomi App Store](https://app.mi.com/game), [Google Play](https://play.google.com/store/apps), [App Store](https://www.apple.com/app-store/). 

All of the files of these triples from application markets are provided in the format of .nt.


### Encyclopedias:
This dataset contains the triples of apps crawled from [Baidu Baike](https://baike.baidu.com), [Toutiao Baike](https://www.baike.com/), [Wikipedia](https://www.wanweibaike.com/).

As the number of Wikipedia is few, we only provide the files of Baidu Baike, Toutiao Baike.


### AppMarket-Alignments:
This dataset contains the alignments of apps, which can share and reuse the description information of apps so as to provide better services based on MAKG for security analysts and users. We utilize two kinds of entity alignment techniques (i.e., Rule miner method, [Knowledge graph embedding-based platform](https://github.com/nju-websoft/OpenEA)) to obtain the best results of them. 

As the number of App Store is fewer than other application markets, we only obtain the alignments among Huawei App Market, Xiaomi App Store, Google Play.


### Extraction-Triples:
This dataset contains the triples extracted from textual descriptions and news related to apps. We utilize three strategies (i.e., Infobox-based Method, Named entity recognition, Relation extraction platforms including [OpenNRE](https://github.com/thunlp/OpenNRE), [DeepKE](https://github.com/zjunlp/deepke), [FewRel](https://github.com/thunlp/FewRel)) and select the best models to extract basic triples. 

## 3. Use-Cases:
We list the main use-cases of [MAKG](http://www.makg.com.cn/) about cybersecurity in our developed [WebSite](http://www.makg.com.cn/). 


- MAKG can provide [semantic retrieval](http://www.makg.com.cn/search) for users and security analysts  For example, if one user queries one app, MAKG can present more comprehensive than application markets to the user. 


- MAKG can link the apps to their appearing textual descriptions (e.g., news) with [entity linking techniques](http://www.makg.com.cn/risk). Benefited from above cases, users can fully understand the information of apps and avoid downloading some invalid apps.

- MAKG can help security analysts to detect some sensitive apps, which own more conditions or plausibility than normal apps that become the hotbeds for related cybercriminals. With the help of comprehensive relations and properties, analysts can define some prior rules or employ more promising algorithms to evaluate the sensitivity and rank them. It can lower the risk of some sensitive apps in advance.

- MAKG can recommend some similar apps for users and security analysts when they request above services. Similarly, if some suitable algorithms are utilized for the recommendation, it can also reduce the potential risks and maintain the security of the Mobile Internet.


## 4. Citation:
If you want to employ this dataset, please cite our paper as follows:

###Normal： 
```
Heng Zhou, Weizhuo Li, Buye Zhang, Qiu Ji, Yiming Tan, and Chongning Na. MAKG: 
A Mobile Application Knowledge Graph for the Research of Cybersecurity. In: Proceedings of China Conference on Knowledge Graph and Semantic Computing, 
Guangzhou, China, Springer, 2021, pp. 321–328.
```


###BibTeX：
```
@inproceedings{MAKG2021, 
author = {Heng Zhou, Weizhuo Li, Buye Zhang, Qiu Ji, Yiming Tan, and Chongning Na}, 
title = {Combining Knowledge Graph Embedding and Network Embedding for 
Detecting Similar Mobile Applications}, 
booktitle = {Proceedings of China Conference on Knowledge Graph and Semantic 
Computing,Guangzhou, China}, 
pages={321--328}, 
year={2021},
publisher={Springer}
}
```
