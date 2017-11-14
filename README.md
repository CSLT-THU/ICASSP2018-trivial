# MACHINE SPEAKER RECOGNITION BASED ON SHORT TRIVIAL EVENTS

Trivial events are ubiquitous in human to human conversations, e.g., cough, laugh and sniff. Compared to regular speech, 
these trivial events are usually short and unclear, thus generally regarded as not speaker discriminative and so are 
largely ignored by present speaker recognition research. However, these trivial events are highly valuable in some 
particular circumstances such as forensic examination, as they are less subjected to intentional change, so can be 
used to discover the genuine speaker from disguised speech.

## DATABASE DESIGN
To collect the data, we designed a mobile application and distributed it to people who agreed to participate. The 
sampling rate of the recordings was set to 16 kHz and the precision of the samples was 8 bits.

We received recordings from 300 participants. The age of the participants ranges from 20 to 60, and most of them are
between 15 and 30. These recordings were manually checked, and those recordings with clear channel effect (noise, 
background babbling and echo) were deleted. After this manual check, recordings from 75 persons were remained.

### CSLT-TRIVIAL-I
The application asked the participants to utter 6 types of trivial events in a random order, and each event 
occurred 10 times randomly. Then, the speech segments were purged and only a single event was retained (e.g., one 
cough or one laugh) in each segment.

Each wav file's name consists of three numbers parted with "_": 
The first one represents the event type: 1--cough, 2--laugh, 16--'Hmm', 17--'Tsk-tsk', 19--'Ahem', 20--'Sniff'
The second one represents person number.
The third one represents segment number.

For the machine test, there are about 260000 trials for each event type.

### CSLT-DISGUISE-I
Before the recording, the participants were instructed to try their best to counterfeit their voices when recording 
the disguise speech. During the recording, the application asked the participants to pronounce 6 sentences. 
Each sentence was spoken twice, one time in the normal style and one time with intentional disguise.

Each wav file's name consists of three numbers parted with "_":
The first one represents the event type: 21--disguise.
The second one represents person number.
The third one represents segment number. (Deserve to be mentioned, the odd segment number is the sentence in normal
style, and the even one is the sentence in disguise. Every two continuous odd-even segments have same texts.)

## Contact

Miao Zhang (zhangmiao@cslt.riit.tsinghua.edu.cn)
Dong Wang (wangdong99@mails.tsinghua.edu.cn)
