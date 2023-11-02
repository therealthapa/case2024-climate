# Task 3 - Shared task on Climate Activism Stance and Hate Event Detection at [CASE 2024](https://emw.ku.edu.tr/case-2024/) #

Hate speech detection and stance detection are some of the most important aspects of event identification during climate change activism events. In the case of hate speech detection, the event is the occurrence of hate speech, the entity is the target of the hate speech, and the relationship is the connection between the two. The hate speech event has targets to which hate is directed. Identification of targets is an important task within hate speech event detection. Additionally, stance event detection is an important part of assessing the dynamics of protests and activisms for climate change. This helps to understand whether the activist movements and protests are being supported or opposed. Thus, in this shared task, we provide three sub-tasks. 

## Sub-task A ##
<b> Hate Speech Detection:</b> Given a text, the goal of this task is to identify whether it contains hate speech or not. The text dataset for this subtask will have binary annotations for the prevalence of hate speech.

## Sub-task B ##
<b> Targets of Hate Speech Detection:</b> The goal of this subtask is to identify the targets of hate speech in a given hateful text. The text is annotated for "individual", "organization", and "community" targets.

## Sub-task C ##
<b> Stance Detection:</b> The goal of this subtask is to identify the stance in a given text. The text is annotated for three different stances namely "support", "oppose", and "neutral".

## Participation ##

In order to participate in the competition, please Join our codalab competition [here](https://codalab.lisn.upsaclay.fr/competitions/16206)

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

## Organizers ##
<ul>
<li> Surendrabikram Thapa (Virginia Tech, USA) </li>
<li> Kritesh Rauniyar (Delhi Technological University, India) </li>
<li> Farhan Ahmad Jafri (Jamia Millia Islamia, India) </li>
<li> Hariram Veeramani (UCLA, USA) </li>
<li> Usman Naseem (James Cook University, Australia) </li>
</ul>

## Contact ##
If there are any questions related to the competition, please contact rauniyark11@gmail.com

## References ##
Will be provided later.
