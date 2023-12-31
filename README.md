# Shared task on Climate Activism Stance and Hate Event Detection at [CASE 2024](https://emw.ku.edu.tr/case-2024/) #

Hate speech detection and stance detection are some of the most important aspects of event identification during climate change activism events. In the case of hate speech detection, the event is the occurrence of hate speech, the entity is the target of the hate speech, and the relationship is the connection between the two. The hate speech event has targets to which hate is directed. Identification of targets is an important task within hate speech event detection. Additionally, stance event detection is an important part of assessing the dynamics of protests and activisms for climate change. This helps to understand whether the activist movements and protests are being supported or opposed. This task will have three subtasks (i) Hate speech identification (ii) Targets of Hate Speech Identification (iii) Stance Detection.

## Sub-task A ##
<b> Hate Speech Detection:</b> Given a text, the goal of this task is to identify whether it contains hate speech or not. The text dataset for this subtask will have binary annotations for the prevalence of hate speech.

## Sub-task B ##
<b> Targets of Hate Speech Detection:</b> The goal of this subtask is to identify the targets of hate speech in a given hateful text. The text is annotated for "individual", "organization", and "community" targets.

## Sub-task C ##
<b> Stance Detection:</b> The goal of this subtask is to identify the stance in a given text. The text is annotated for three different stances namely "support", "oppose", and "neutral".

## Participation ##

In order to participate in the competition, please Join our codalab competition [here](https://codalab.lisn.upsaclay.fr/competitions/16206)

**Training Data:**

| SubTask | Link |
|----------|----------|
| SubTask-A | [here](https://drive.google.com/file/d/1bjqQ7CHIGZpTB0aDinkry5sfCAUCMyx_/view?usp=sharing) |
| SubTask-B | [here](https://drive.google.com/file/d/16eaYd4ks4zyIIOHM91edZndrt9ogGBsu/view?usp=sharing) |
| SubTask-C | [here](https://drive.google.com/file/d/16gdvDM3jTIaym_oe79Di15ByCUwQMXOm/view?usp=sharing) |

**Eval Data:**


| SubTask | Link (index-tweet)| Link (index-label)|
|----------|----------|----------|
| SubTask-A | [here](https://drive.google.com/file/d/18SQ7JXd9tJQByUeQRYJz5CdUIJWqDoCk/view?usp=sharing) | [here](https://drive.google.com/file/d/1EaYACFTY9-LL0rux8Pl0ZxnErybpdRsC/view?usp=sharing) | 
| SubTask-B | [here](https://drive.google.com/file/d/1Scwkb6kI3CG-zzHbkWri1lcypUc68Zcz/view?usp=sharing) |[here](https://drive.google.com/file/d/15hdfMZshigvS1IpyA1bEVN6B65bZdw1g/view?usp=sharing) |
| SubTask-C | [here](https://drive.google.com/file/d/1s-iV5Qpp9--eoxqrjYhoi2LPL47W1MNw/view?usp=sharing) | [here](https://drive.google.com/file/d/1m_FXICq6PmPzO3SjTHqWuV8s-XMiRlYk/view?usp=sharing) |


**Test Data:**

| SubTask | Link |
|----------|----------|
| SubTask-A | [here](https://drive.google.com/file/d/1bZ8GglFqdDhRk_9CbHlTyI0qlYAlNc5h/view?usp=sharing) |
| SubTask-B | [here](https://drive.google.com/file/d/1OJmz9SULtxQDhnNXOiBZIoftmtqxNckj/view?usp=sharing) |
| SubTask-C | [here](https://drive.google.com/file/d/1TRocNnYOMq_5SzC5sf8iTT2SN7MCJ7Hz/view?usp=sharing) |

## Dataset ## 
All the text has a unique identifier called "index". The labels for training data are given along with the dataset. For evaluation and testing, the submission format is mentioned below.

## Evaluation ## 

The results are only accepted in codalab. The submission will be evaluated with a f1-score.

The script takes one prediction file as the input. Your submission file must be a JSON file which is then zipped. We will only take the first file in the zip folder, so do not zip multiple files together. 


For subtask A, the final prediction submissions should be like the following. Make sure that your hate label is given as "1" and the non-hate label is given as "0".

<b>IMPORTANT:</b> The index in JSON should be in ascending order.
```python
{"index": 15636, "prediction": 0}
{"index": 16006, "prediction": 1}
{"index": 19818, "prediction": 0}
```

Similarly, for subtask B, the final prediction submissions should be like the following. Make sure that your individual, organization, and community labels are given as "1", "2", and "3" respectively.

<b>IMPORTANT:</b> The index in JSON should be in ascending order.
```python
{"index": 13943, "prediction": 1}
{"index": 15708, "prediction": 3}
{"index": 16692, "prediction": 2}
```


Similarly, for the subtask C, the final prediction submissions should be like the following. Make sure that your support, oppose, and neutral labels are given as "1", "2", and "3" respectively.

<b>IMPORTANT:</b> The index in JSON should be in ascending order.
```python
{"index": 10433, "prediction": 1}
{"index": 18276, "prediction": 3}
{"index": 20346, "prediction": 2}
```

## Publication ##
Participants in the Shared Task are expected to submit a paper to the workshop. Submitting a paper is not mandatory for participating in the Shared Task. Papers must follow the EACL 2024 workshop submission instructions and will undergo regular peer review. Their acceptance will not depend on the results obtained in the shared task but on the quality of the paper. Authors of accepted papers will be informed about the evaluation results of their systems prior to the paper submission deadline (see the important dates). All the accepted papers will be published in ACL Anthology.

## Invitation for Special Issue ##
Top-performing teams and best models will be invited for a special issue in journals (T.B.D.).

## Timeline of the Events ##
<ul>

<li>Training & Evaluation data available: Nov 1, 2023 </li>

<li>Test data available: Nov 30, 2023 </li>

<li>Test start: Nov 30, 2023 </li>

<li>Test end: Jan 7, 2024 </li>

<li>System Description Paper submissions due: Jan 13, 2024 </li>

<li>Notification to authors after review: Jan 26, 2024 </li>

<li>Camera ready: Jan 30, 2024 </li>

<li>CASE Workshop: 21-22 Mar, 2024 </li>
</ul>

## Organizers ##
<ul>
<li> Surendrabikram Thapa (Virginia Tech, USA) </li>
<li> Kritesh Rauniyar (Delhi Technological University, India) </li>
<li> Farhan Ahmad Jafri (Jamia Millia Islamia, India) </li>
<li> Ali Hürriyetoğlu (KNAW Humanities Cluster DHLab, Netherlands) </li>
<li> Hariram Veeramani (UCLA, USA) </li>
<li> Usman Naseem (James Cook University, Australia) </li>
</ul>

## Contact ##
If there are any questions related to the competition, please contact rauniyark11@gmail.com

## References ##
Will be provided later.
