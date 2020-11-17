---
layout: default
---

<!-- <h1 align='center'><font size='10'> Emotion Transfer Based on Global Style Tokens and Adversarial Training </font></h1>

<center>Pengfei Wu, Junjie Pan, Junhui Zhang, Chenchang Xu, Lin Wu, Xiang Yin, Zejun Ma</center>
 -->
# Abstract

In expressive speech synthesis, there are high requirements for emotion interpretation. However, it is time-consuming to acquire emotional audio corpus for arbitrary speakers due to their deduction ability. This paper proposes a Tacotron-based model using Global Style Tokens (GSTs) to transfer the emotion control ability from one speaker with multiple emotions to another. An adversarial training mechanism and a speaker classifier are introduced to eliminate the speaker-related information in tokens. Experimental results show that the proposed method can achieve the goal and the synthesized speech outperforms significantly on naturalness than the Tacotron baseline.        

### Fine-grained emotion transfer using proposed method after paper submission*
The emotional speaker(s1) and non-emotional speaker(s2) are both female. We transfer fine-grained emotion from s1 to s2 using proposed method.

|emotion|sample|
| --- | --- |
| neutral | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/fine-grain/neutral.wav"></audio> |
| happy | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/fine-grain/happy.wav"></audio> |
| sad | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/fine-grain/sad.wav"></audio> |
| angry | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/fine-grain/angry.wav"></audio> |
| scare | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/fine-grain/scare.wav"></audio> |
| surprise | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/fine-grain/surprise.wav"></audio> |
| hate | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/fine-grain/hate.wav"></audio> |

# Audio Samples
## 1. AB test
### a. Performance on *neutral*
We first show the performance of systems on *neutral*. 

| system| Sample1 | Sample2|
| --- | --- | --- |
| baseline | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/1_neutral/baseline/1.wav"></audio> | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/1_neutral/baseline/2.wav"></audio> |
| ET-Taco | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/1_neutral/ET_Taco/1.wav"></audio> | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/1_neutral/ET_Taco/2.wav"></audio> |
| ET-GST | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/1_neutral/GST/1.wav"></audio> | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/1_neutral/GST/2.wav"></audio> |
| ET-GST-SC | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/1_neutral/GST_SC/1.wav"></audio> | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/1_neutral/GST_SC/2.wav"></audio> |
| ET-GST-SC-no-DA | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/1_neutral/GST_SC_no_DA/1.wav"></audio> | <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/1_neutral/GST_SC_no_DA/2.wav"></audio> |

### b. Comparsion of ET-Taco and ET-GST
As mentioned in the paper, ET-GST is much stable than ET-Taco.

<table>
<thead>
  <tr>
    <th>system</th>
    <th>ET_Taco</th>
    <th>ET_GST</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td rowspan="5">Samples</td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/2_ET_Taco_GST/ET_Taco/1.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/2_ET_Taco_GST/ET_GST/1.wav"></audio> </td>
  </tr>
  <tr>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/2_ET_Taco_GST/ET_Taco/2.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/2_ET_Taco_GST/ET_GST/2.wav"></audio> </td>
  </tr>
  <tr>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/2_ET_Taco_GST/ET_Taco/3.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/2_ET_Taco_GST/ET_GST/3.wav"></audio> </td>
  </tr>
  <tr>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/2_ET_Taco_GST/ET_Taco/4.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/2_ET_Taco_GST/ET_GST/4.wav"></audio> </td>
  </tr>
  <tr>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/2_ET_Taco_GST/ET_Taco/5.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="audios/ab/2_ET_Taco_GST/ET_GST/5.wav"></audio> </td>
  </tr>
</tbody>
</table>


## 2. Emotion perception

<table>
<thead>
  <tr>
    <th>systems</th>
    <th>ET_Taco</th>
    <th>ET_GST</th>
    <th>ET_GST_SC</th>
  </tr>
</thead>
<tbody>
  <!-- neutral -->
  <tr>
    <td rowspan="2">neutral</td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_Taco/neutral/1.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST/neutral/1.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST_SC/neutral/1.wav"></audio> </td>
  </tr>
  <tr>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_Taco/neutral/2.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST/neutral/2.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST_SC/neutral/2.wav"></audio> </td>
  </tr>
  <!-- happy -->
  <tr>
    <td rowspan="2">happy</td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_Taco/happy/1.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST/happy/1.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST_SC/happy/1.wav"></audio> </td>
  </tr>
  <tr>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_Taco/happy/2.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST/happy/2.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST_SC/happy/2.wav"></audio> </td>
  </tr>
  <!-- angry -->
  <tr>
    <td rowspan="2">angry</td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_Taco/angry/1.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST/angry/1.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST_SC/angry/1.wav"></audio> </td>
  </tr>
  <tr>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_Taco/angry/2.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST/angry/2.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST_SC/angry/2.wav"></audio> </td>
  </tr>
  <!-- sad -->
  <tr>
    <td rowspan="2">sad</td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_Taco/sad/1.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST/sad/1.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST_SC/sad/1.wav"></audio> </td>
  </tr>
  <tr>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_Taco/sad/2.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST/sad/2.wav"></audio> </td>
    <td> <audio id="audio" controls="" preload="none" style="height: 40px;width: 185px"> <source id="wav" src="audios/emotion_perception/ET_GST_SC/sad/2.wav"></audio> </td>
  </tr>
</tbody>
</table>

