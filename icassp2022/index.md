---
layout: default
---

<h1 align='center'><font size='10'> Cross-speaker Emotion Transfer Based on Speaker Condition Layer Normalization and Semi-Supervised Training in Text-To-Speech </font></h1>

<center>Pengfei Wu, Junjie Pan, Chenchang Xu, Junhui Zhang, Lin Wu, Xiang Yin, Zejun Ma</center>

# Abstract

In expressive speech synthesis, there are high requirements for emotion interpretation. However, it is time-consuming to acquire emotional audio corpus for arbitrary speakers due to their deduction ability. In response to this problem, this paper proposes a cross-speaker emotion transfer method that can realize the transfer of emotions from source speaker to target speaker. A set of emotion tokens is firstly defined to represent various categories of emotions. They are trained to be highly correlated with corresponding emotions for controllable synthesis by cross-entropy loss and semi-supervised training strategy. Meanwhile, to eliminate the down-gradation to the timbre similarity from cross-speaker emotion transfer, speaker condition layer normalization is implemented to model speaker characteristics. 
Experimental results show that the proposed method outperforms the multi-reference based baseline in terms of timbre similarity, stability and emotion perceive evaluations.       

###  Reference speech of *source speaker* and *target speaker*

<table>
    <tr>
        <th>emotion</th>
        <th>source speaker</th>
        <th>target speaker</th>
    </tr>
    <tr>
        <th>
            neutral
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/reference/source/neutral.wav"></audio>
        </td>
        <td rowspan="7"> 
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/reference/target/1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/reference/target/2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/reference/target/3.wav"></audio>
        </td>
    </tr>
    <tr>
        <th>
            happy
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/reference/source/happy.wav"></audio>
        </td>
    </tr>
    <tr>
        <th>
            sad
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/reference/source/sad.wav"></audio>
        </td>
    </tr>
    <tr>
        <th>
            angry
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/reference/source/angry.wav"></audio>
        </td>
    </tr>
    <tr>
        <th>
            surprise
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/reference/source/surprise.wav"></audio>
        </td>
    </tr>
    <tr>
        <th>
            scare
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/reference/source/scare.wav"></audio>
        </td>
    </tr>
    <tr>
        <th>
            hate
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/reference/source/hate.wav"></audio>
        </td>
    </tr>
</table>


# Synthesized samples
<table>
    <tr>
        <th>
            emotion
        </th>
        <th>
            baseline
        </th>
        <th>
            M1
        </th>
        <th>
            M2
        </th>
        <th>
            proposed
        </th>
    </tr>
    <tr>
        <th>
            neutral
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/neutral_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/neutral_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/neutral_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/neutral_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/neutral_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/neutral_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/neutral_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/neutral_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/neutral_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/neutral_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/neutral_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/neutral_3.wav"></audio>
        </td>
    </tr>
    <tr>
        <th>
            happy
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/happy_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/happy_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/happy_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/happy_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/happy_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/happy_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/happy_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/happy_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/happy_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/happy_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/happy_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/happy_3.wav"></audio>
        </td>
    </tr>
    <tr>
        <th>
            sad
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/sad_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/sad_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/sad_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/sad_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/sad_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/sad_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/sad_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/sad_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/sad_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/sad_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/sad_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/sad_3.wav"></audio>
        </td>
    </tr>
    <tr>
        <th>
            angry
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/angry_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/angry_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/angry_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/angry_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/angry_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/angry_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/angry_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/angry_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/angry_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/angry_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/angry_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/angry_3.wav"></audio>
        </td>
    </tr>
    <tr>
        <th>
            surprise
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/surprise_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/surprise_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/surprise_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/surprise_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/surprise_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/surprise_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/surprise_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/surprise_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/surprise_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/surprise_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/surprise_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/surprise_3.wav"></audio>
        </td>
    </tr>
    <tr>
        <th>
            scare
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/scare_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/scare_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/scare_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/scare_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/scare_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/scare_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/scare_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/scare_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/scare_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/scare_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/scare_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/scare_3.wav"></audio>
        </td>
    </tr>
    <tr>
        <th>
            hate
        </th>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/hate_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/hate_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/baseline/hate_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/hate_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/hate_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M1/hate_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/hate_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/hate_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/M2/hate_3.wav"></audio>
        </td>
        <td>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/hate_1.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/hate_2.wav"></audio>
            <audio id="audio" controls="" preload="none" style="height: 40px"> <source id="wav" src="demos/proposed/ratio_1.0/hate_3.wav"></audio>
        </td>
    </tr>
</table>
