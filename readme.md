<h1 align="center"><strong>OMG3D: 3D Object Manipulation in a Single Image Using Generative Models</strong></h1>

<!-- 
| ![GIF 1](demo/videos/gif_application/box_walk.gif) | ![GIF 2](demo/videos/gif_application/box_greet.gif) | ![GIF 3](demo/videos/gif_application/plane.gif) | ![GIF 4](demo/videos/gif_application/pumpkin.gif) | ![GIF 5](demo/videos/gif_application/elephant.gif) |
|-----------------------------|----------------------------|----------------------------|----------------------------|----------------------------| -->

<!-- 第一行：显示四个 GIF -->
<!-- | ![GIF 1](demo/videos/gif_application/michelle.gif) | ![GIF 2](demo/videos/gif_application/box_greet.gif) | ![GIF 3](demo/videos/gif_application/plane.gif) | ![GIF 4](demo/videos/gif_application/box_walk.gif) |
|-----------------------------|----------------------------|----------------------------|----------------------------|


|              ![GIF 5](demo/videos/gif_application/pumpkin.gif)             |           ![GIF 6](demo/videos/gif_application/pete.gif)          |           ![GIF 7](demo/videos/gif_application/elephant.gif)          |
|:----------------------------------:|:----------------------------------:|:----------------------------------:| -->

<!-- 第一行：四个 GIF -->
| ![GIF 1](demo/videos/gif_application/pumpkin.gif) | ![GIF 2](demo/videos/gif_application/box_greet.gif) | ![GIF 3](demo/videos/gif_application/plane.gif) | ![GIF 4](demo/videos/gif_application/box_walk.gif) |
|-----------------------------|----------------------------|----------------------------|----------------------------|

<!-- 第二行：三张 GIF 居中，两侧空单元格保持等宽 -->
|                             | ![GIF 5](demo/videos/gif_application/michelle.gif) | ![GIF 6](demo/videos/gif_application/pete.gif) | ![GIF 7](demo/videos/gif_application/elephant.gif) |
|:---------------------------:|:----------------------------:|:----------------------------:|:---------------------------:|



<p align="center"><b>Applications of OMG3D.</b></p>

<hr>

<section class="section hero is-light is-small">
  <div class="container is-max-desktop">
    <!-- Abstract. -->
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 align="center" class="title is-3">Abstract</h2>
        <div class="content has-text-justified">
          <p>
            Object manipulation in images aims to not only edit the object presentation but 
            also gift objects with motion. Previous methods encountered challenges in concurrently 
            handling static editing and dynamic motion applications, while also struggling to 
            achieve realism in object appearance and scene lighting. In this work, we introduce OMG3D, 
            a novel framework that integrates the precise geometric control with the generative power 
            of diffusion models, thus achieving significant enhancements in visual performance. 
            Our framework converts 2D objects into 3D, enabling user-directed modifications and 
            lifelike motions at the geometric level. To address texture realism, we propose CustomRefiner, 
            a texture refinement module that pretrain a customized diffusion model to align the 
            style and perspectives of coarse renderings with the original image. Additionally, 
            we introduce IllumiCombiner, an lighting processing module that estimates and adjusts 
            background lighting to match human visual perception, resulting in more realistic 
            illumination. Extensive experiments demonstrate the outstanding visual performance of
            our approach in both static and dynamic scenarios. Remarkably, all these steps
            can be done using one NVIDIA 3090. The code and project page will be released
            upon acceptance of the paper.
          </p>
        </div>
      </div>
    </div>
    
</section>
<hr>

<!-- ![Alt text](demo/images/pipeline.jpg)

<p align="center"><b>Model structure of our model, OMG3D.</b></p>

![Alt text](demo/images/edit_compare.jpg)
<p align="center"><b>Comparison with other image edit methods. </b></p>
 -->
<p align="center"><b>Model structure of our model, OMG3D.</b></p>
<p align="center">
  <img src="demo/images/pipeline.jpg" alt="Model structure of our model, OMG3D" width="1200">
</p>

<p align="center"><b>Comparison with other image edit methods.</b></p>
<p align="center">
  <img src="demo/images/edit_compare.jpg" alt="Comparison with other image edit methods" width="1200">
</p>


<hr>

<div align="center">
Text Description: A rotated pumpkin jumping on a stump.

<table>
  <!-- 第一行 -->
  <tr>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/pumpkin_dc.gif" alt="GIF 1" width="500"><br>
    <p>By DynamiCrafter</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/pumpkin_is.gif" alt="GIF 2" width="500"><br>
    <p>By Image Sculpting</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/pumpkin_our.gif" alt="GIF 3" width="500"><br>
    <p>Ours</p>
  </td>
</tr>

<!-- 第二行 -->
<tr>
  <td colspan="3" align="center">
    <div style="display: flex; justify-content: center; max-width: 1500px;">
      <div style="text-align: center; width: 33.33%;">
        <img src="demo/videos/gif_comparison/pumpkin_pika.gif" alt="GIF 4" width="500"><br>
        <p>By Pika Video Model</p>
      </div>
      <div style="text-align: center; width: 33.33%; margin-left: 20px;">
        <img src="demo/videos/gif_comparison/pumpkin_svd.gif" alt="GIF 5" width="500"><br>
        <p>By SVD</p>
      </div>
    </div>
  </td>
</tr>



</table>

<br>
Text Description: An elephant is walking on the ground.

<table align="center">
  <!-- 第一行 -->
   <tr>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/elephant_dc.gif" alt="GIF 1" width="500"><br>
    <p>By DynamiCrafter</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/elephant_is.gif" alt="GIF 2" width="500"><br>
    <p>By Image Sculpting</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/elephant_our.gif" alt="GIF 3" width="500"><br>
    <p>Ours</p>
  </td>
</tr>

<!-- 第二行 -->
<tr>
  <td colspan="3" align="center">
    <div style="display: flex; justify-content: center; max-width: 1500px;">
      <div style="text-align: center; width: 33.33%;">
        <img src="demo/videos/gif_comparison/elephant_pika.gif" alt="GIF 4" width="500"><br>
        <p>By Pika Video Model</p>
      </div>
      <div style="text-align: center; width: 33.33%; margin-left: 20px;">
        <img src="demo/videos/gif_comparison/elephant_svd.gif" alt="GIF 5" width="500"><br>
        <p>By SVD</p>
      </div>
    </div>
  </td>
</tr>
</table>

<br>
Text Description: A boxtoy greeting on the keyboard.

<table align="center">
  <!-- 第一行 -->
   <tr>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/box_dc.gif" alt="GIF 1" width="500"><br>
    <p>By DynamiCrafter</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/box_is.gif" alt="GIF 2" width="500"><br>
    <p>By Image Sculpting</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/box_our.gif" alt="GIF 3" width="500"><br>
    <p>Ours</p>
  </td>
</tr>

<!-- 第二行 -->
<tr>
  <td colspan="3" align="center">
    <div style="display: flex; justify-content: center; max-width: 1500px;">
      <div style="text-align: center; width: 33.33%;">
        <img src="demo/videos/gif_comparison/box_pika.gif" alt="GIF 4" width="500"><br>
        <p>By Pika Video Model</p>
      </div>
      <div style="text-align: center; width: 33.33%; margin-left: 20px;">
        <img src="demo/videos/gif_comparison/box_svd.gif" alt="GIF 5" width="500"><br>
        <p>By SVD</p>
      </div>
    </div>
  </td>
</tr>
  </tr>
</table>

<br>
<p><b>Comparison with other image animation methods.</b></p>
</center>
