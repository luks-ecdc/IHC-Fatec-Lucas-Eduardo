# IHC-Fatec-Lucas-Eduardo
Este projeto consiste em mudar um pouco a questão monótoma de ensino nas empresas, tirando aquele modo 
antigo de livretos e materiais impressos, se dá inicio à tecnologia de AR/VR (Realidade Aumentada/Realidade Virtual).

Utilizando o CodePen ( https://codepen.io/xlucasFatec/pen/YzKomgX?editors=1000 ), vamos utilizar uma chamada de objeto 
HIRO
(https://jeromeetienne.github.io/AR.js/data/images/HIRO.jpg) e 

Kanji (https://www.solutionfactory.in/resources/images/posts/5/kanji.png) da câmera do celular ou notebook para iniciar a projeção AR de uma furadeira e um tripé de furadeira.

# Iniciando o Projeto

Utilizando o CodePen (https://codepen.io/xlucasFatec/pen/ExYqNaM?editors=1000) iniciarei com um teste básico utilizando o Hiro ( https://jeromeetienne.github.io/AR.js/data/images/HIRO.jpg) para projetar um cubo amarelo.

![modelo3d teste](https://user-images.githubusercontent.com/37638307/66013316-23066500-e4a1-11e9-9977-761825313856.png)

# Code3dbox HTML

```
<!doctype HTML>
<html>
<script src="https://aframe.io/releases/0.9.2/aframe.min.js"></script>
<script src="https://raw.githack.com/jeromeetienne/AR.js/1.7.5/aframe/build/aframe-ar.js"></script>
  <body style='margin : 0px; overflow: hidden;'>
    <a-scene embedded arjs>
  	<a-marker preset="hiro">
            <a-box position='0 0.5 0' material='color: yellow;'></a-box>
  	</a-marker>
  	<a-entity camera></a-entity>
    </a-scene>
  </body>
</html>
```

>> O que falta fazer? <<
* Incluir eventos de toque/ clique.
* Incluir a interação do modelo 3D da furadeira com o modelo 3D do tripé.
* Incluir um tutorial escrito e áudio. 
