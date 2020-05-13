# Dirichlet Process
### Summary
<font size="3">   
Brief introduction and implementations of related concepts to Dirichlet Processes: GEM distribution, Polya Urn, Chinese restaurant process, Stick-Breaking construction, and Posterior of a DP. 
<br></br>
<ol>
  <li><b>Griffiths-Engen-McCloskey (GEM) Distribution:</b></li>
      <ol>
          <li>Definition.</li>
          <li>Function to construct samples <img src="https://render.githubusercontent.com/render/math?math=\pi%20=%20(\pi_{1},%20\pi_{2},%20...)"> </li>
          <li>Function to construct sample distribution <img src="https://render.githubusercontent.com/render/math?math=\pi%20\sim%20GEM(\alpha)"> </li>
          <li>GEM Figures for different <img src="https://render.githubusercontent.com/render/math?math=\alpha"> values:</li>
              <ol>
                  <li>Figure 1: Distribution of weight values for each dimension <img src="https://render.githubusercontent.com/render/math?math=\pi_{i}"> of <img src="https://render.githubusercontent.com/render/math?math=\pi%20\sim%20GEM(\alpha)">, shows the behavior of <img src="https://render.githubusercontent.com/render/math?math=\pi"> for different <img src="https://render.githubusercontent.com/render/math?math=\alpha"> values</li>
                  <li>Figure 2: Sample vectors <img src="https://render.githubusercontent.com/render/math?math=\pi"> and the decreasing trend in average of the weights as we increase dimension <img src="https://render.githubusercontent.com/render/math?math=\pi_{k}"> </li>
                  <li>Figure 3: Stick representation for 15 <img src="https://render.githubusercontent.com/render/math?math=\pi"> samples, from the whole probability vector <img src="https://render.githubusercontent.com/render/math?math=\pi\%20(\sum_{k}%20\pi_{k}=1)"> show each dimension weight with a different color. Another way of representing Figure 1.</li>
              </ol>
      </ol>   
  <li><b>Polya urn.</b></li>
      <ol>
          <li>Definition.</li>
          <li>Function to model Polya urn.</li>
          <li>Figure 1: Distribution of independent samples of Polya urns, only high number of draws show to be distributed as a Beta distribution.</li>
      </ol>   
  <li><b>Chinese Restaurant process.</b></li>
      <ol>
          <li>Definition.</li>
          <li>Function to model table assignations. </li>
          <li>Function to construct the Chinese restaurant process</li>
          <li>Figure 1: CRP mean <img src="https://render.githubusercontent.com/render/math?math=E[|\varrho|/%20n,%20\alpha]"> and variance <img src="https://render.githubusercontent.com/render/math?math=Var[|\varrho|/%20n,%20\alpha]"> on number of tables for different <img src="https://render.githubusercontent.com/render/math?math=\pi%20\sim%20GEM(\alpha)"> values.</li>
      </ol>   
  <li><b>Dirichlet Process:</b>.</li>
      <ol>
          <li>Definitions:</li>
              <ol>
                  <li>Stick-breaking representation.</li>
                  <li>Ferguson's definition.</li>
              </ol>
          <li>Function to construct samples using the stick-breaking representation: <img src="https://render.githubusercontent.com/render/math?math=G%20=%20\sum_{k=1}^{\infty}%20\pi_{k}\delta(\theta,\theta_{k})"> </li>
          <li>Function to construct sample distribution <img src="https://render.githubusercontent.com/render/math?math=G%20\sim%20DP(\alpha,%20H)"> </li>
          <li>DP Figures for different <img src="https://render.githubusercontent.com/render/math?math=\alpha"> values:</li>
              <ol>
                  <li>Figure 1: Draws from a DP using the stick-breaking representation.</li>
                  <li>Figure 2: Visualization of a DP through Ferguson's definition: <img src="https://render.githubusercontent.com/render/math?math=E[G(A)]"> , <img src="https://render.githubusercontent.com/render/math?math=Var[G(A)]">, and the impact of the concentration parameter <img src="https://render.githubusercontent.com/render/math?math=\pi%20\sim%20GEM(\alpha)">.</li>
                  <li>Figure 3: Visualization of a DP through Ferguson's definition: Cumulative distributions of the random probability measure <img src="https://render.githubusercontent.com/render/math?math=G"> and the base measure <img src="https://render.githubusercontent.com/render/math?math=H">.</li>
              </ol>
          <li><b>Posterior DP:</b></li>
              <ol>
                  <li>Posterior construction through stick-breaking.</li>
                  <li>Function to construct the DP posterior from obseravations.</li>
                  <li>Figure 1: DP posterior visualizations for different number of observations of an 'assumed true' DP posterior and <img src="https://render.githubusercontent.com/render/math?math=\alpha,%20H"> values in the prior.</li>
              </ol>
      </ol>
  <li><b>Notebooks:</b></li>
  <ol>
    <li>[DP Visualizations](https://github.com/AdalbertoCq/Dirichlet_processes/blob/master/dirichlet_process.ipynb).</li>
    <li>Variational Inference [GMM](https://github.com/AdalbertoCq/Dirichlet_processes/blob/master/VariationalInference_GMM.ipynb) and [DPMM](https://github.com/AdalbertoCq/Dirichlet_processes/blob/master/Varaitional%20Inference%20DPMM.ipynb).</li>
  </ol> 
</ol>
</font>

A couple of DP Visualizations, a larger set and explanations in the [notebook](https://github.com/AdalbertoCq/Dirichlet_processes/blob/master/dirichlet_process.ipynb):
<img src="https://github.com/AdalbertoCq/Dirichlet_processes/blob/master/images/dp_visual/dp_visualization_alpha_100.png" width="1000">

<img src="https://github.com/AdalbertoCq/Dirichlet_processes/blob/master/images/dp_visual/cumulative_G_alpha_10.png" width="1000">

<img src="https://github.com/AdalbertoCq/Dirichlet_processes/blob/master/images/dp_draw/dp_draw_deltas_alpha_100.png" width="1000">

<img src="https://github.com/AdalbertoCq/Dirichlet_processes/blob/master/images/post_dp/cumulative_posterior_G_alpha_10_N_03_10_obs_alpha_obs_10_N05.png" width="1000">
