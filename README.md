# DSLAB_project
Project DS LAB course

Project based on a speech recognition task. The goal is to correct classify the content of audio files.

The dataset consists in a collection of audio file in a WAV format. Each record is characterized by several
attributes. The following is a short description for each of them.
• path: the path of the audio file.
• speakerId: the id of the speaker.
• action: the type of action required through the intent.
• object: the device involved by intent.
• Self-reported fluency level: the speaking fluency of the speaker.
• First Language spoken: the first language spoken by the speaker.
• Current language used for work/school: the main language spoken by the speaker during daily activities.
• gender: the gender of the speaker.
• ageRange: the age range of the speaker.

An intent is given by the combination of an action with an object, therefore the information in the two
respective columns must be combined to obtain the label to be used to address this task. The way this
information should be combined is a simple string concatenation (e.g., if the action is “increase” and the
object is “volume”, the corresponding intent will be “increasevolume”).

Within the archive, you will find the following elements:
• audio: a folder containing all the audio files in WAV format.
• development.csv (development set): a comma-separated values file containing the records from
the development set. This portion does have the action and object columns, which you should use
to obtain the labels to train and validate your models.
• evaluation.csv (evaluation set): a comma-separated values file containing the records corresponding
to the evaluation set. This portion does not have the action and object columns.
• sample_submission.csv: a sample submission file.

The aim is to build a classification pipeline to predict the intent expressed in each audio recording.
