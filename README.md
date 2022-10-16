# stablediff

<center>Toward Generations of New Gacha Images for Better h(hyeok)-index</center>  

from https://github.com/nonmetal/stable-diffusion-webui (deprecated)

## Style Transfer with Modified Layer Structure

1. Generation from base model

| `looking at viewer, portrait, 1girl, blonde hair`<br> *(default negative prompts)* |
|---|
| ![](https://static-cdn.jtvnw.net/jtv_user_pictures/2bf27338-cc3a-4f35-af09-7e925395da4b-profile_image-300x300.png) ![](https://static-cdn.jtvnw.net/jtv_user_pictures/2bf27338-cc3a-4f35-af09-7e925395da4b-profile_image-300x300.png#style=max-width:20px;vertical-align:middle) ![](https://static-cdn.jtvnw.net/jtv_user_pictures/2bf27338-cc3a-4f35-af09-7e925395da4b-profile_image-300x300.png#style=max-width:20px;vertical-align:middle)| 

2. Hypernetwork training with Modified Layer Structure

<table>
  <tr>
  <th colspan="3">`looking at viewer, portrait, 1girl, blonde hair`<br> *(default negative prompts)*</th>
  </tr>
  <tr>
    <th> `nn.Linear(), depth == 2` (base)</th>
    <th> `nn.Linear(), depth == 6` </th>
    <th> `nn.conv1d(), depth == 2` </th>    
  </tr>
</table>
