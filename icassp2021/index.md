---
layout: default
---

<!-- <h1 align='center'><font size='10'> Emotion Transfer Based on Global Style Tokens and Adversarial Training </font></h1>

<center>Pengfei Wu, Junjie Pan, Junhui Zhang, Chenchang Xu, Lin Wu, Xiang Yin, Zejun Ma</center>
 -->
# Abstract

In expressive speech synthesis, there are high requirements for emotion interpretation. However, it is time-consuming to acquire emotional audio corpus for arbitrary speakers due to their deduction ability. This paper proposes a Tacotron-based model using Global Style Tokens (GSTs) to transfer the emotion control ability from one speaker with multiple emotions to another. An adversarial training mechanism and a speaker classifier are introduced to eliminate the speaker-related information in tokens. Experimental results show that the proposed method can achieve the goal and the synthesized speech outperforms significantly on naturalness than the Tacotron baseline.        


# Audio Samples

## Natural 

here put some nautral audios

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
## Converted Samples

<!-- * **M1:** BASE1
* **M2:** BASE2
* **M3:** BASE3
* **M4:** BASE3 + ME
* **M5:** BASE3 + ME + SC
* **M6:** BASE3 + ME + SC + MS **\(our proposed model\)** -->

<!-- #### Target Female

| | F1 | F2 | F3 | M1 | M2 | M3 |
| --- | --- | --- | --- | --- | --- | --- |
| BASE1 | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m1/F_CDF008_XT_097_023-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m1/F_F007_WXR_011_026-01.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m1/F_F008_ZYF_008_009-00.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m1/M_CDM008_GG_99_032-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m1/M_M003_CYC_018_020-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m1/M_M005_S_013_023-06.wav"></audio> |
| BASE2 | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m2/F_CDF008_XT_097_023-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m2/F_F007_WXR_011_026-01.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m2/F_F008_ZYF_008_009-00.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m2/M_CDM008_GG_99_032-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m2/M_M003_CYC_018_020-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m2/M_M005_S_013_023-06.wav"></audio> |
| BASE3 | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m3/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m3/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m3/F_F008_ZYF_008_009-00_F_F008_ZYF_008_009-00.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m3/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m3/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m3/M_M005_S_013_023-06_M_M005_S_013_023-06.npy.wav"></audio> |
| **Proposed** | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m6/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m6/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m6/F_F008_ZYF_008_009-00_F_F008_ZYF_008_009-00.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m6/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m6/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m6/M_M005_S_013_023-06_M_M005_S_013_023-06.npy.wav"></audio> |

#### Target Male

| | F1 | F2 | F3 | M1 | M2 | M3 |
| --- | --- | --- | --- | --- | --- | --- |
| BASE1 | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m1/F_CDF008_XT_097_023-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m1/F_F007_WXR_011_026-01.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m1/F_F008_ZYF_008_009-00.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m1/M_CDM008_GG_99_032-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m1/M_M003_CYC_018_020-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m1/M_M005_S_013_023-06.wav"></audio> |
| BASE2 | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m2/F_CDF008_XT_097_023-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m2/F_F007_WXR_011_026-01.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m2/F_F008_ZYF_008_009-00.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m2/M_CDM008_GG_99_032-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m2/M_M003_CYC_018_020-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m2/M_M005_S_013_023-06.wav"></audio> |
| BASE3 | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m3/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m3/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m3/F_F008_ZYF_008_009-00_F_F008_ZYF_008_009-00.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m3/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m3/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m3/M_M005_S_013_023-06_M_M005_S_013_023-06.npy.wav"></audio> |
| **Proposed** | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m6/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m6/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m6/F_F008_ZYF_008_009-00_F_F008_ZYF_008_009-00.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m6/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m6/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m6/M_M005_S_013_023-06_M_M005_S_013_023-06.npy.wav"></audio> |



## Ablation Tests

#### Target Female

| | F1 | F2 | M1 | M2 |
| --- | --- | --- | --- | --- |
| BASE3 | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m3/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m3/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m3/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m3/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> |
| + ME | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m4/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m4/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m4/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m4/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> |
| + SC | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m5/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m5/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m5/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m5/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> |
| + MS **\(Proposed\)** | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m6/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m6/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m6/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/m6/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> |

#### Target Male

| | F1 | F2 | M1 | M2 |
| --- | --- | --- | --- | --- |
| BASE3 | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m3/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m3/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m3/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m3/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> |
| + ME | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m4/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m4/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m4/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m4/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> |
| + SC | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m5/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m5/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m5/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m5/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> |
| + MS **\(Proposed\)** | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m6/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m6/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m6/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/m6/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> |


## Noise Robustness Tests

#### source SNR = 15.30

| | F1 | F2 | M1 | M2 |
| --- | --- | --- | --- | --- |
| Source | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/source_noise1/F_CDF008_XT_097_023-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/source_noise1/F_F007_WXR_011_026-01.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/source_noise1/M_CDM008_GG_99_032-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/source_noise1/M_M003_CYC_018_020-02.wav"></audio> |
| Target Female | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/noise1/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/noise1/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/noise1/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/noise1/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> |
| Target Male | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/noise1/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/noise1/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/noise1/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/noise1/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> |

#### source SNR = 8.18

| | F1 | F2 | M1 | M2 |
| --- | --- | --- | --- | --- |
| Source | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/source_noise2/F_CDF008_XT_097_023-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/source_noise2/F_F007_WXR_011_026-01.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/source_noise2/M_CDM008_GG_99_032-02.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/source_noise2/M_M003_CYC_018_020-02.wav"></audio> |
| Target Female | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/noise2/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/noise2/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/noise2/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/BB/noise2/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> |
| Target Male | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/noise2/F_CDF008_XT_097_023-02_F_CDF008_XT_097_023-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/noise2/F_F007_WXR_011_026-01_F_F007_WXR_011_026-01.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/noise2/M_CDM008_GG_99_032-02_M_CDM008_GG_99_032-02.npy.wav"></audio> | <audio id="audio" controls="" preload="none" style="width: 140px;height: 50px"> <source id="wav" src="audios/AM2/noise2/M_M003_CYC_018_020-02_M_M003_CYC_018_020-02.npy.wav"></audio> | -->

