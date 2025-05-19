<h1 align="center"><strong>OMINI: Unlocking Object Manipulation in a Single Image</strong></h1>

<p align="center"><b>Applications of OMINI.</b></p>
<!-- 第一行：四个 GIF -->

|![GIF 1](demo/videos/gif_application/elephant_walk2.gif) | ![GIF 2](demo/videos/gif_application/boxtoy_our.gif) |![GIF 3](demo/videos/gif_application/woodenman_our2.gif) |![GIF 4](demo/videos/gif_application/pumpkin_our.gif) |
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
            Unlocking versatile object manipulation—from appearance editing to full animation—directly from a static image remains a challenging problem. Existing methods often struggle to simultaneously support both visual modification and realistic animation, while also falling short in preserving object fidelity and realistic scene illumination. In this work, we introduce OMINI, a unified framework that addresses these challenges through two complementary strategies. First, to support both static editing and dynamic animation, OMINI operates directly on 3D object geometry thereby sharing a unified representation across tasks, enabling consistent appearance under varying poses and motions during manipulation. Second, to improve fidelity in both object appearance and scene illumination, we incorporate two dedicated modules: CGTRefiner, which refines rendered views using a concept-specific diffusion model and optimizes the UV texture map via differentiable rasterization; and IHLCorrector, which adjusts estimated lighting based on object-level color priors to enhance realism. Extensive experiments demonstrate that OMINI achieves superior performance in both static and dynamic settings, producing high-quality and visually consistent results. Notably, the entire pipeline operates efficiently on a single NVIDIA RTX 3090 GPU. Code and models will be released upon paper acceptance.
          </p>
        </div>
      </div>
    </div>
    
</section>
<hr>

<p align="center"><b>Model structure of our model, OMINI.</b></p>
<p align="center">
  <img src="demo/images/model_pipeline.png" alt="Model structure of our model, OMINI" width="1200">
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
    <img src="demo/videos/gif_comparison/elephant/elephant_walk2.gif" alt="GIF 3" width="200"><br>
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
    <img src="demo/videos/gif_comparison/woodenman/woodenman_our2.gif" alt="GIF 3" width="200"><br>
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
