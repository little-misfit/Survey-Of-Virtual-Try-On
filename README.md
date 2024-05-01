# Image-Based Virtual Try-On: A Survey

This repository corresponds to the paper [**"Image-Based Virtual Try-On: A Survey"**](http://arxiv.org/abs/2311.04811).
If you find our survey useful for your research, please cite the following paper:

```
@misc{Image_Based_Virtual_Try-On_A_Survey,
      title={Image-Based Virtual Try-On: A Survey}, 
      author={Dan Song and Xuanpu Zhang and Juan Zhou and Weizhi Nie and Ruofeng Tong and An-An Liu},
      year={2023},
      eprint={2311.04811},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```


## ⏲️ The Timeline of virtual try-on papers

We have listed some of the most representative works in the field of virtual fitting from recent years.

![Time-line](https://github.com/fengyun691340/Survey-Of-Virtual-Try-On/blob/main/Time_line3.png)


## 🔍 Experiments

### Data prepare

To ensure a fair test for each model, we produced a high-resolution (1024x768) version of the [**VITON**](https://github.com/xthan/VITON). dataset, following the data preprocessing method of [**VITON-HD**](https://github.com/shadow2496/VITON-HD).

- 14221 train
  - images
  - cloth
  - segmentation
  - densepose
  - keypoints
  - agnostic-person
- 2032 test

High-resolution [**Dataset**](https://pan.baidu.com/s/1Gf82137uCTKecF_h6f2eaA?pwd=mq5i).

### Experiment Results

We evaluated the models through two perspectives: visual results and quantitative metrics.

Visual results of VITON:
![visual results of VITON](https://github.com/fengyun691340/Survey-Of-Virtual-Try-On/blob/main/keshitu_viton2.png)


Visual results of VITON-HD:
![visual results of VITON-HD](https://github.com/fengyun691340/Survey-Of-Virtual-Try-On/blob/main/keshitu_hd.jpg)

More visual results from [**here(BaiduYunDownload:pdub)**](https://pan.baidu.com/s/1YnyqAAHpQRDnTp5jObzpSg?pwd=pdub).

Quantitative metrics of VITON:
SSIM:
![SSIM](readme/plot_SSIM.png)
FID:
![FID](readme/plot_FID.png)
LPIPS:
![LPIPS](readme/plot_LPIPS.png)
Semantic Score:
![Semantic Score](readme/plot_Clip.png)


Quantitative metrics of VITON-HD:
SSIM:
![SSIM](https://github.com/fengyun691340/Survey-Of-Virtual-Try-On/blob/main/plot_FID2_hd.png)
FID:
![FID](https://github.com/fengyun691340/Survey-Of-Virtual-Try-On/blob/main/plot_FID2_hd.png)
LPIPS:
![LPIPS](https://github.com/fengyun691340/Survey-Of-Virtual-Try-On/blob/main/plot_LPIPS2_hd.png)
Semantic Score:
![Semantic Score](https://github.com/fengyun691340/Survey-Of-Virtual-Try-On/blob/main/plot_Clip2_hd.png)



## Papers & Data Sets

<details><summary>Papers</summary>
<table class="tg">
<thead>
  <tr>
    <th class="tg-baqh" align="center" rowspan="2">model</th>
    <th class="tg-0lax" align="center" rowspan="2">Release Time</th>
    <th class="tg-0lax" align="center" rowspan="2">Paper</th>
    <th class="tg-0lax" align="center" rowspan="2">Code</th>
  </tr>
  <tr>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-baqh" align="center">CAGAN</td>
    <td class="tg-0lax" align="center">2017</td>
    <td class="tg-0lax" align="center"><a href="https://arxiv.org/abs/1709.04695">Paper</a></td>
    <td class="tg-0lax" align="center">-</td>
  </tr>


</tbody>
</table>
</details>

<details><summary>Data Sets</summary>
<table class="tg">
<thead>
  <tr>
    <th class="tg-baqh" align="center" rowspan="2">Data set</th>
    <th class="tg-0lax" align="center" rowspan="2">Release Time</th>
    <th class="tg-0lax" align="center" rowspan="2">Resolution</th>
	<th class="tg-0lax" align="center" rowspan="2">Quantity Train/Test</th>
    <th class="tg-0lax" align="center" rowspan="2">Link</th>
  </tr>
  <tr>
  </tr>
</thead>

<tbody>
  <tr>
    <td class="tg-baqh" align="center">VITON</td>
    <td class="tg-0lax" align="center">2018</td>
    <td class="tg-0lax" align="center">256*192</td>
	<td class="tg-0lax" align="center">14221/2032</td>
    <td class="tg-0lax" align="center"><a href="https://github.com/xthan/VITON">Link</a></td>
  </tr>
  <tr>
    <td class="tg-baqh" align="center">MPV</td>
    <td class="tg-0lax" align="center">2019</td>
    <td class="tg-0lax" align="center">256*192</td>
	<td class="tg-0lax" align="center">52236/10544</td>
    <td class="tg-0lax" align="center"><a href="https://pan.baidu.com/s/1VZSJg5KRYKRCn8DzIyPOLQ?pwd=ipno">Collected by us(BaiduYunDownload:ipno)</a></td>
  </tr>
  <tr>
    <td class="tg-baqh" align="center">DeepFashion</td>
    <td class="tg-0lax" align="center">2016</td>
    <td class="tg-0lax" align="center">1101*750</td>
	<td class="tg-0lax" align="center">52712/*</td>
    <td class="tg-0lax" align="center"><a href="https://github.com/yumingj/DeepFashion-MultiModal">Link</a></td>
  </tr>
  <tr>
    <td class="tg-baqh" align="center">VITON-HD</td>
    <td class="tg-0lax" align="center">2021</td>
    <td class="tg-0lax" align="center">1024*768</td>
	<td class="tg-0lax" align="center">11647/2032</td>
    <td class="tg-0lax" align="center"><a href="https://github.com/shadow2496/VITON-HD">Link</a></td>
  </tr>
  <tr>
    <td class="tg-baqh" align="center">ESF</td>
    <td class="tg-0lax" align="center">2022</td>
    <td class="tg-0lax" align="center">512*512</td>
	<td class="tg-0lax" align="center">170000/10000</td>
    <td class="tg-0lax" align="center"><a href="https://github.com/RuiLiFeng/Deep-Generative-Projection">Link</a></td>
  </tr>
  <tr>
    <td class="tg-baqh" align="center">DressCode</td>
    <td class="tg-0lax" align="center">2022</td>
    <td class="tg-0lax" align="center">1024*768</td>
	<td class="tg-0lax" align="center">48392/5400</td>
    <td class="tg-0lax" align="center"><a href="https://github.com/aimagelab/dress-code">Link</a></td>
  </tr>
  <tr>
    <td class="tg-baqh" align="center">VITON(After Processing)</td>
    <td class="tg-0lax" align="center">2022</td>
    <td class="tg-0lax" align="center">1024*768</td>
	<td class="tg-0lax" align="center">14221/2032</td>
    <td class="tg-0lax" align="center"><a href="https://pan.baidu.com/s/1Gf82137uCTKecF_h6f2eaA?pwd=mq5i">BaiduYunDownload:mq5i</a></td>
  </tr>

  

</tbody>
</table>
</details>


## Acknowledgments

We acknowledge the contributions of [**awesome-virtual-try-on**](https://github.com/minar09/awesome-virtual-try-on) to the community, which saved us time in collecting literature.

