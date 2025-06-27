<h1>Two-Stage CNN-LSTM</h1>
<p><em>Learning the spatio-temporal link between wind and significant wave height&nbsp;(Hs)</em></p>

<p>
  This repository provides the Python implementation for predicting significant wave height from wind fields with a two-stage deep-learning pipeline that combines Convolutional Neural Networks&nbsp;(CNN) and Long Short-Term Memory&nbsp;(LSTM) units. The full approach is described in:
</p>

<blockquote>
  <p>
    Obakrim, S. <em>et&nbsp;al.</em> “Learning the spatiotemporal relationship between wind and significant wave height using deep learning,”
    <em>Environmental Data Science</em>, 2022.
    <a href="https://doi.org/10.1017/eds.2022.35">doi:10.1017/eds.2022.35</a>
  </p>
</blockquote>

<h2>Data sources</h2>
<table>
  <thead>
    <tr>
      <th>Variable</th>
      <th>Archive</th>
      <th>Link</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Significant wave height&nbsp;(Hs)</strong></td>
      <td>HOMERE hindcast (Ifremer)</td>
      <td><a href="https://marc.ifremer.fr/produits/rejeu_d_etats_de_mer_homere">Link</a></td>
    </tr>
    <tr>
      <td><strong>Wind fields</strong></td>
      <td>Climate Forecast System Reanalysis (CFSR)</td>
      <td><a href="https://climatedataguide.ucar.edu/climate-data/climate-forecast-system-reanalysis-cfsr">Link</a></td>
    </tr>
  </tbody>
</table>

<p>
  Pre-processed datasets used in the paper can be downloaded directly
  <a href="https://drive.google.com/drive/folders/1SIXYRXIpoegZ_bTLsvmr1g77GLMnMWy_?usp=sharing">here</a>.
</p>

<h2>Method overview</h2>
<ol>
  <li><strong>CNN stage</strong> — extracts spatial features from consecutive wind-field snapshots.</li>
  <li><strong>LSTM stage</strong> — learns temporal dependencies and predicts the corresponding Hs time series.</li>
</ol>

<p style="text-align:center;">
  <img src="https://github.com/SaidObakrim/Two-stage-CNN-LSTM-/blob/main/cnn_architicture.png" alt="Model architecture">
</p>


<h2>Citation</h2>
<pre><code>@article{obakrim2022twostage,
  title  = {Two-stage CNN–LSTM for learning the spatio-temporal relationship between wind and significant wave height},
  author = {Obakrim, S. and others},
  journal= {Environmental Data Science},
  year   = {2022},
  doi    = {10.1017/eds.2022.35}
}
</code></pre>

</body>
</html>
