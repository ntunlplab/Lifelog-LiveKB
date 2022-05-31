# LiveKB [laɪv kei bi]
A Lifelog Dataset for Personal Knowledge Base Construction
# Introduction
People often forget something in the daily life, thus information recall support for people at the right time and at the right place is emerging. Constructing personal knowledge base for individuals is important for the application of memory recall and living assistance. We collect 18 users who set their tweets as public and posted tweets ranged from 2009 to 2017. We aim to extract life events from tweets shared on Twitter, and construct personal knowledge bases of individuals.

# Format
Each entry in the JSON format is consisted of "tweet_id" (the id of the tweet), "hasEvent" (annotated result), and "triples" (annotated result).

"triples" is consist of "eventType", "frame", "subject", "predicate", "object", and "time" of each life event.

"eventType" denote the explicitness of the life event. "frame" in "triples" is consist of frame name for each predicate and semantic roles following the definition of [Chinese FrameNet](https://github.com/ntunlplab/FrameNet-CFN-Lex).

# Example
```yaml
        {'hasEvent': 'with-life-event',
        'triples': [{'eventType': 'explicit',
                     'frame': {'frame_element': [{'frame_element_name': 'Entity',
                                                  'frame_element_type': 'core',
                                                  'index': None,
                                                  'token': '@User'},
                                                 {'frame_element_name': 'Location',
                                                  'frame_element_type': 'core',
                                                  'index': '3-5',
                                                  'token': '将军岭'}],
                               'frame_name': 'Presence',
                               'index': '2',
                               'target': '@'},
                     'object': '将军岭',
                     'predicate': '@',
                     'subject': '@User',
                     'time': '發文時間'},
                    {'eventType': 'implicit',
                     'frame': {'frame_element': [{'frame_element_name': 'Entity',
                                                  'frame_element_type': 'core',
                                                  'index': None,
                                                  'token': '@User'},
                                                 {'frame_element_name': 'Location',
                                                  'frame_element_type': 'core',
                                                  'index': '0-1',
                                                  'token': '新店'}],
                               'frame_name': 'Presence',
                               'index': None,
                               'target': '在'},
                     'object': '新店',
                     'predicate': '在',
                     'subject': '@User',
                     'time': '發文時間'}],
        'tweet_id': '239534741467045888'}
```
*There is a mistake in our paper: the numbers of the tweets with and without life event are 8,915 and 16,429, respectively.*
# Download
Please write us an email with the agreement. Click here to download the agreement of LiveKB.

Email Address: azyen@nlg.csie.ntu.edu.tw

# How to Cite the Corpus
Please cite the following papers when referring to the LiveKB in academic publications and papers.

An-Zi Yen, Hen-Hsen Huang, and Hsin-Hsi Chen. 2019. Personal Knowledge Base Construction from Text-based Lifelogs. In Proceedings of the 42nd International ACM SIGIR Conference on Research and Development in Information Retrieval, 185-194.
An-Zi Yen, Hen-Hsen Huang, and Hsin-Hsi Chen. 2019. Multimodal Joint Learning for Personal Knowledge Base Construction from Twitter-Based Lifelogs. In Information Processing & Management. DOI: https://doi.org/10.1016/j.ipm.2019.102148.
