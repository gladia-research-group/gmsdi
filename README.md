# Generalized Multi-Source Inference for Text Conditioned Music Diffusion Models

 * **Paper:** ***Generalized Multi-Source Inference for Text Conditioned Music Diffusion Models***  <br/><br/>
 * **Authors:** Emilian Postolache, Giorgio Mariani, Luca Cosmo, Emmanouil Benetos, Emanuele Rodolà  <br/><br/>
 * **Abstract:** Multi-Source Diffusion Models (MSDM) allow for compositional musical generation tasks: generating a set of coherent sources, creating accompaniments, and performing source separation. Despite their versatility, they require estimating the joint distribution over the sources, necessitating pre-separated musical data, which is rarely available, and fixing the number and type of sources at training time. This paper generalizes MSDM to arbitrary time-domain diffusion models conditioned on text embeddings. These models do not require separated data as they are trained on mixtures, can parameterize an arbitrary number of sources, and allow for rich semantic control. We propose an inference procedure enabling the coherent generation of sources and accompaniments. Additionally, we adapt the Dirac separator of MSDM to perform source separation. We experiment with diffusion models trained on Slakh2100  and MTG-Jamendo, showcasing competitive generation and separation results in a relaxed data setting.


## Source Imputation (a.k.a. Partial Generation)
Given a source stem as input (e.g. drums), the neural model generates accompanying instruments:

### Piano

| Original Source | Generated accompaniment| Final Mix |
| :----------: | :----------: | :----------: |
|<audio controls preload="none"><source src="media/inpainting/piano2/1_cond.mp3" type="audio/mpeg"> </audio> |   <audio controls preload="none"><source src="media/inpainting/piano2/1_mix.mp3" type="audio/mpeg"> </audio>|   <audio controls preload="none"><source src="media/inpainting/piano2/1_mix.mp3" type="audio/mpeg"> </audio>|

### Guitar

| Original Source | Generated accompaniment| Final Mix |
| :----------: | :----------: | :----------: |
|<audio controls preload="none"><source src="media/inpainting/guitar/1_cond.mp3" type="audio/mpeg"> </audio> |   <audio controls preload="none"><source src="media/inpainting/guitar/1_mix.mp3" type="audio/mpeg"> </audio>|<audio controls preload="none"><source src="media/inpainting/guitar/1_mix.mp3" type="audio/mpeg"> </audio>|

### Bass

| Original Source | Generated accompaniment| Final Mix |
| :----------: | :----------: | :----------: |
|<audio controls preload="none"><source src="media/inpainting/bass/1_cond.mp3" type="audio/mpeg"> </audio> |   <audio controls preload="none"><source src="media/inpainting/bass/1_mix.mp3" type="audio/mpeg"> </audio>| <audio controls preload="none"><source src="media/inpainting/bass/1_mix.mp3" type="audio/mpeg"> </audio>|

### Drums

| Original Source | Generated accompaniment| Final Mix |
| :----------: | :----------: | :----------: |
|<audio controls preload="none"><source src="media/inpainting/drums/1_cond.mp3" type="audio/mpeg"> </audio> |   <audio controls preload="none"><source src="media/inpainting/drums/1_mix.mp3" type="audio/mpeg"> </audio>|  <audio controls preload="none"><source src="media/inpainting/drums/1_mix.mp3" type="audio/mpeg"> </audio>|

<br/><br/>
