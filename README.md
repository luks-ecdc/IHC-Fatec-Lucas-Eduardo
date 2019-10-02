# IHC-Fatec-Lucas-Eduardo
Este projeto consiste em mudar um pouco a questão monótoma de ensino nas empresas, tirando aquele modo 
antigo de livretos e materiais impressos, se dá inicio à tecnologia de AR/VR (Realidade Aumentada/Realidade Virtual).

Utilizando o CodePen ( https://codepen.io/ ), vamos utilizar uma chamada da imagem hiro e kanji

# HIRO
![HIRO](https://user-images.githubusercontent.com/37638307/66013913-619d1f00-e4a3-11e9-8acb-737d1dc064fb.jpg) 

 

# Kanji
![kanji](https://user-images.githubusercontent.com/37638307/66013856-33b7da80-e4a3-11e9-909e-38a0b029908c.png)

da câmera do celular ou notebook para iniciar a projeção AR de uma furadeira e um tripé de furadeira.

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
# Teste com Hiro e Kanji

Acrescentando o 
``` <script src="'http://examples.org/kanji.patt'"></script>```

e

```
<a-marker preset='kanji'>
      <a-box position='0 0.5 0' material='color: red;'></a-box>
</a-marker> 
```
    
 podemos utilizar 2 marcadores de projeção.

![teste com 2](https://user-images.githubusercontent.com/37638307/66015023-619f1e00-e4a7-11e9-8381-faec157d4829.png)

# Implementando um modelo 3D da furadeira
 Nessa parte foi utilizada um modelo pego no (https://sketchfab.com/)
 o modelo gltf foi colocado em um repositório do Github (https://github.com/xluminatus/drill)
 Utilizando o CodePen (https://codepen.io/xlucasFatec/pen/YzKomgX?editors=1000) 
 inserimos a chamada do link do Raw do model.dae no marker Hiro
 
 ``` <html>
    <script src="https://aframe.io/releases/0.8.2/aframe.min.js"></script>
    <script src="https://cdn.rawgit.com/jeromeetienne/AR.js/1.7.8/aframe/build/aframe-ar.js"></script>
      <body style='margin : 0px; overflow: hidden;'>
        <a-scene embedded arjs>
            
        <a-marker preset="hiro">
            <a-entity collada-model="url(https://raw.githubusercontent.com/xluminatus/drill/master/model.dae)"
                      rotation = "-90 0 0"
                      scale = "3 3 3"></a-entity>
        </a-marker>
          
         <a-entity camera></a-entity>
        </a-scene>
      </body>
    </html>
    
```
![drill](https://user-images.githubusercontent.com/37638307/66042538-1579cb00-e4f3-11e9-90ce-2bdcccb40d8a.png)


# O que falta fazer? <<
* incluir um modelo de furadeira sem tripé 
* Incluir o modelo 3D de tripé 
* Incluir eventos de toque/ clique.
* Incluir a interação do modelo 3D da furadeira com o modelo 3D do tripé.
* Incluir um tutorial escrito e áudio. 
