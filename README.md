# Task 4 - Shared task on Multimodal Hate Speech Event Detection at [CASE 2024](https://emw.ku.edu.tr/case-2024/) #

Hate speech detection and stance detection are some of the most important aspects of event identification during climate events. In the case of hate speech detection, the event is the occurrence of hate speech, the entity is the target of the hate speech, and the relationship is the connection between the two. Given a text, this task aims to automatically identify the hate speech, targets of hate speech, and stance. This task will have three subtasks.

Details 

## Sub-task A ##
<b> Hate Speech Detection:</b> The goal of this task is to identify whether the given text contains hate speech or not. The text, which are the dataset for this subtask, will have annotations for the prevalence of hate speech.


## Sub-task B ##
<b> Targets of Hate Speech Detection:</b> The goal of this subtask is to identify the targets of hate speech in a given hateful text. The text are annotated for "individual", "organization", and "community" targets.


## Sub-task C ##
<b> Stance Detection:</b> The goal of this subtask is to identify the stance in a given text. The text are annotated for "support", "oppose", and "neutral" stance.


## Participation ##

In order to participate in the competition, please Join our codalab competition [here](https://codalab.lisn.upsaclay.fr/competitions/13087)

## Dataset ## 
All the text have a unique identifier called "index". The labels for training data are organized in the folder provided. For evaluation and testing, the submission format is mentioned below.

## Evaluation ## 

The results are only accepted in codalab. The submission will be evaluated with a f1-score.

The script takes one prediction file as the input. Your submission file must be a JSON file which is then zipped. We will only take the first file in the zip folder, so do not zip multiple files together. 

<b>IMPORTANT:</b> The index (text ID) in json should be in ascending order.

For subtask A, the final prediction submissions should be like the following. Make sure that your hate label is given as "1" and non-hate label is given as "0".

```python
{"index": 16006, "prediction": 1}
{"index": 19818, "prediction": 0}
{"index": 15636, "prediction": 0}
```

Similarly, for the subtask B, the final prediction submissions should be like the following. Make sure that your individual, organization, and community labels are given as "1", "2", and "3" respectively.

```python
{"index": 13943, "prediction": 1}
{"index": 16692, "prediction": 2}
{"index": 15708, "prediction": 3}
```

<b>IMPORTANT:</b> The index (text ID) in json should be in ascending order.


## Publication ##
Participants in the Shared Task are expected to submit a paper to the workshop. Submitting a paper is not mandatory for participating in the Shared Task. Papers must follow the EACL 2024 workshop submission instructions and will undergo regular peer review. Their acceptance will not depend on the results obtained in the shared task but on the quality of the paper. Authors of accepted papers will be informed about the evaluation results of their systems prior to the paper submission deadline (see the important dates). All the accepted papers will be published in ACL Anthology.

## Invitation for Special Issue ##
Top-performing teams and best models will be invited for a special issue in journals (T.B.D.).

## Timeline of the Events ##

## Organizers ##
<ul>
<li> Surendrabikram Thapa (Virginia Tech, USA) </li>
<li> Hariram Veeramani (UCLA, USA) </li>
<li> Kritesh Rauniyar (Delhi Technological University, India) </li>
<li> Farhan Ahmad Jafri (Jamia Millia Islamia, India) </li>
<li> Usman Naseem (James Cook University, Australia) </li>
</ul>

## Contact ##
If there are any questions related to the competition, please contact rauniyark11@gmail.com

## References ##
