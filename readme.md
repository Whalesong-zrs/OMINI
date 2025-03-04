<h1 align="center"><strong>3D Object Manipulation in a Single Image Using Generative Models</strong></h1>

<p align="center"><b>Applications of OMG3D.</b></p>
<!-- 第一行：四个 GIF -->

|![GIF 1](demo/videos/gif_application/elephant_our.gif) | ![GIF 2](demo/videos/gif_application/boxtoy_our.gif) |![GIF 3](demo/videos/gif_application/woodenman_our.gif) |![GIF 4](demo/videos/gif_application/pumpkin_our.gif) |
|:---------------------------:|:----------------------------:|:----------------------------:|:---------------------------:|

<!-- 第二行：三张 GIF 居中，两侧空单元格保持等宽 -->
|![GIF 5](demo/videos/gif_application/michelle.gif) | ![GIF 6](demo/videos/gif_application/pete.gif) | ![GIF 7](demo/videos/gif_application/plane.gif) |![GIF 8](demo/videos/gif_application/dog.gif) |
|:---------------------------:|:----------------------------:|:----------------------------:|:---------------------------:|


<hr>

<section class="section hero is-light is-small">
  <div class="container is-max-desktop">
    <!-- Abstract. -->
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 align="center" class="title is-3">Abstract</h2>
        <div class="content has-text-justified">
          <p>
            Object manipulation in images aims not only to edit the 
            object appearances but also to animate objects. Previous
            methods faced challenges in simultaneously handling static
            editing and dynamic generation, while also struggling to
            achieve fidelity in object appearance and scene lighting.
            In this work, we introduce OMG3D, a novel framework
            that combines precise geometric control with the generative 
            power of diffusion models, thus achieving significant
            improvements in visual performance. Our framework first
            converts 2D objects into 3D, enabling user-directed modifications
            and lifelike motion at the geometric level. To
            address texture realism, we propose CustomRefiner, a texture
            refinement module that pre-trains a customized diffusion model, 
            aligning the details and style of coarse renderings from the
            rough 3D model with the original image, further refining the texture.
            Additionally, we introduce IllumiCombiner, a lighting processing module
            that estimates and corrects background lighting to match human visual
            perception, resulting in more realistic shadow effects. Extensive
            experiments demonstrate the outstanding visual performance of 
            our approach in both static and dynamic scenarios. Remarkably, 
            all of these steps can be executed on a single NVIDIA 3090. The
            code and project will be released upon the acceptance of the paper.
          </p>
        </div>
      </div>
    </div>
    
</section>
<hr>

<p align="center"><b>Model structure of our model, OMG3D.</b></p>
<p align="center">
  <img src="demo/images/pipeline.png" alt="Model structure of our model, OMG3D" width="1200">
</p>

<p align="center"><b>Comparison with other image edit methods.</b></p>
<p align="center">
  <img src="demo/images/edit_compare.png" alt="Comparison with other image edit methods" width="1200">
</p>

<hr>

<p align="center"><b>Comparison with other image animation methods.</b></p>

<table align="center">
  <tr>
    <div align="center">
      <span style="max-width: 800px; color: #B8860B; font-size: 14px;">
        Text Description: An elephant is walking on the ground.
      </span>
    </div>
    <td align="center" style="width: 33.33%;">
      <img src="demo/videos/gif_comparison/elephant/elephant_pika.gif" alt="GIF 1" width="200"><br>
      <p>By Pika</p>
    </td>
    <td align="center" style="width: 33.33%;">
      <img src="demo/videos/gif_comparison/elephant/elephant_dc.gif" alt="GIF 2" width="200"><br>
      <p>By DynamiCrafter</p>
    </td>
    <td align="center" style="width: 33.33%;">
      <img src="demo/videos/gif_comparison/elephant/elephant_cogvideox.gif" alt="GIF 3" width="200"><br>
      <p>CogVideoX</p>
    </td>
  </tr>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/elephant/elephant_wan.gif" alt="GIF 1" width="200"><br>
    <p>By Wan</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/elephant/elephant_is.gif" alt="GIF 2" width="200"><br>
    <p>By ImgScu</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/elephant/elephant_our.gif" alt="GIF 3" width="200"><br>
    <p>Ours</p>
  </td>
</table>

<table align="center">
  <tr>
    <div align="center">
      <span style="max-width: 800px; color: #3498db; font-size: 14px;">
        Text Description: A boxtoy greets and waves its hand.
      </span>
    </div>
    <td align="center" style="width: 33.33%;">
      <img src="demo/videos/gif_comparison/boxtoy/boxtoy_pika.gif" alt="GIF 1" width="200"><br>
      <p>By Pika</p>
    </td>
    <td align="center" style="width: 33.33%;">
      <img src="demo/videos/gif_comparison/boxtoy/boxtoy_dc.gif" alt="GIF 2" width="200"><br>
      <p>By DynamiCrafter</p>
    </td>
    <td align="center" style="width: 33.33%;">
      <img src="demo/videos/gif_comparison/boxtoy/boxtoy_cogvideox.gif" alt="GIF 3" width="200"><br>
      <p>CogVideoX</p>
    </td>
  </tr>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/boxtoy/boxtoy_wan.gif" alt="GIF 1" width="200"><br>
    <p>By Wan</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/boxtoy/boxtoy_is.gif" alt="GIF 2" width="200"><br>
    <p>By ImgScu</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/boxtoy/boxtoy_our.gif" alt="GIF 3" width="200"><br>
    <p>Ours</p>
  </td>
</table>

<table align="center">
  <tr>
    <div align="center">
      <span style="max-width: 800px; color: #8B7500; font-size: 14px;">
        Text Description: A woodenman sits and cheers.
      </span>
    </div>
    <td align="center" style="width: 33.33%;">
      <img src="demo/videos/gif_comparison/woodenman/woodenman_pika.gif" alt="GIF 1" width="200"><br>
      <p>By Pika</p>
    </td>
    <td align="center" style="width: 33.33%;">
      <img src="demo/videos/gif_comparison/woodenman/woodenman_dc.gif" alt="GIF 2" width="200"><br>
      <p>By DynamiCrafter</p>
    </td>
    <td align="center" style="width: 33.33%;">
      <img src="demo/videos/gif_comparison/woodenman/woodenman_cogvideox.gif" alt="GIF 3" width="200"><br>
      <p>CogVideoX</p>
    </td>
  </tr>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/woodenman/woodenman_wan.gif" alt="GIF 1" width="200"><br>
    <p>By Wan</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/woodenman/woodenman_is.gif" alt="GIF 2" width="200"><br>
    <p>By ImgScu</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/woodenman/woodenman_our.gif" alt="GIF 3" width="200"><br>
    <p>Ours</p>
  </td>
</table>

<table align="center">
  <tr>
    <div align="center">
      <span style="max-width: 800px; color: #8b0000c4; font-size: 14px;">
        Text Description: A rotated pumpkin jumps on a stump.
      </span>
    </div>
    <td align="center" style="width: 33.33%;">
      <img src="demo/videos/gif_comparison/pumpkin/pumpkin_pika.gif" alt="GIF 1" width="200"><br>
      <p>By Pika</p>
    </td>
    <td align="center" style="width: 33.33%;">
      <img src="demo/videos/gif_comparison/pumpkin/pumpkin_dc.gif" alt="GIF 2" width="200"><br>
      <p>By DynamiCrafter</p>
    </td>
    <td align="center" style="width: 33.33%;">
      <img src="demo/videos/gif_comparison/pumpkin/pumpkin_cogvideox.gif" alt="GIF 3" width="200"><br>
      <p>CogVideoX</p>
    </td>
  </tr>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/pumpkin/pumpkin_wan.gif" alt="GIF 1" width="200"><br>
    <p>By Wan</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/pumpkin/pumpkin_is.gif" alt="GIF 2" width="200"><br>
    <p>By ImgScu</p>
  </td>
  <td align="center" style="width: 33.33%;">
    <img src="demo/videos/gif_comparison/pumpkin/pumpkin_our.gif" alt="GIF 3" width="200"><br>
    <p>Ours</p>
  </td>
</table>

</center>
