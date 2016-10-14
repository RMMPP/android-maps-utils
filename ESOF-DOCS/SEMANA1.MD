Este projecto consiste numa biblioteca open source que pode ser utilizada por aplicações que fazem uso da API do Google Maps, principalmente no sistema operativo para dispositivos móveis, neste caso Android.

O objectivo é da biblioteca é acrescentar utilitários (add-ons), partindo da API existente da Google, entre eles salientamos:

##### Marker clustering 
— permite dividir o mapa em quadrados com um determinado tamanho, o tamanaho depende do nível de zoom utilizado, e agrupa os marcadores nos quadradro;
##### Heat maps 
— Uma camada mapa de calor é a visualização que demonstra a intensidade dos dados em determinados pontos geográficos. Quando uma camada de calor é activada um sobreposição colorida é exibida sobre o mapa;
##### IconGenerator 
— Permite criar e gerir icons contendo texto com info sob a forma de uma janela;
##### Poly decoding and encoding 
— Codigo compacto para caminhos e interoperabilidade com o serviço web da Maps API. As polylinhas na API do google são formadas por um conjunto de refências que indentificam a latitude e longitude de um determinado ponto. Através do "encoding"  compactamos uma série de coordenadas (latitude longitude), que designamos por caminho, numa única string.
##### Spherical geometry 
— for example: computeDistance, computeHeading, computeArea
##### KML 
— faz display da KML data
##### GeoJSON 
— faz display e personaliza GeoJSON data

O programa aparenta ter como objectivo fazer a manutenção da biblioteca e mantê-la relevante para que outros developpers a possam utilizar nas suas próprias aplicações. Esta biblioteca não tem cliente final, ou seja, o processo de validação é feito por utilizadores que decidam usar a biblioteca nos seus próprios projectos e no caso de haver falta de funcionalidades ou imperfeições podem ou nao ser comunicadas aos autores via Git.

Na procura do processo de desenvolvimento entramos em contacto com Maciej Górski e com Chris Broadfoot. Chris foi o autor inicial do projecto mas infelizmente não conseguimos que ele nos respondesse. O Maciej embora tenha respondido informou-nos que já não se encontra envolvido com o projecto e diferiu-nos para o Chris. Estamos ainda a espera de resposta.

Por observação do projecto podemos inferir que o processo que mais assemelha ao desenvolvimento, seja o processo de desenvolvimento e entrega incremental. Dizemos isto pois o programa vai avançando por versões onde os diferentes utilizadores vão submetendo pequenas adições e correcções às diferentas facetas do programa que são posteriormente revistas e aprovadas pelos autores.
Mas não existe muita documentação a que possamos recorrer para saber a lista de tarefas a desenvolver. Existe apenas um template para submeter issues através do github. Com isso também não nós é possível identificar o ponto actual do projecto. Inicialmente a biblioteca foi começada por "Broady" que nos primeiros meses fez grande parte do desenvolvimento, deixando pouca documentação. Em seguida "microcat" tambem contribuiu com bastante depois das contribuições de "broady" baixarem, mas não existe documentação.

A biblioteca foi construida por individuos que aparentemente pouco comunicaram entre eles e foram fazendo as alterações que achavam pertinentes. Isto sugere que houve uma falta de planeamento e estruturação bem como uma falta de documentação do processo. Existem muitas acções correctivas e adaptativas pois existe uma lista de "issues" (problemas) que os utilizadores podem ver e participar na sua correcção. Efetivamente isto mostra um nível muito básico de organização e muito pouco eficiente.

Após a verificação dos commits efectuados podemos verificar que não existe planeamento temporal, nem prazo pré-definidos.

Sugerimos a implementação das seguintes medidas:
- Uma lista de actividades a desenvolver, bem como o ponto actual do desenvolvimento;
- Criação de um log de activades desenvolvidas, com eventuais pontos a melhorar;
- Neste momento baseado na falta de documentação, não existe uma lista funcionalidades implementadas CORRETAMENTE, o utilizador tem de instalar a aplicação e testa-la de forma a ver o que funciona. O projecto aparenta estar actualmente num estado de erro. A lista de funcionalidades esperadas não nos fornece a certeza de quais a funcionalidades actualmente operacionais. Trata-se portanto de documentação mais apropriada para os estágios finais do desenvolvimento do software. Existe no entanto, um video protagonizado pelo principal autor deste projecto, no qual dá alguns exemplos de utilização mas, novamente, trata-se de documentação mais adequada a um produto finalizado.
- Apontar um manager ao projecto que faz um controlo de qualidade interativo. A biblioteca encontra-se pouco supervisionada. É necessario a existência de alguém que teste as funcionalidades periodicamente e que mantenha um log de funcionamento, ou seja, se a aplicação funciona como esperado ou se existem falhas. O responsavel deve então documentar as falhas em diferentes cenários de arquitetura, bem como os seus sucessos. (p.ex: funciona em androids de versão x para cima e as funcinalidades GeoJSON não funciona em certos modelos).

Jocosamente, a grande temática do processo de desenvolvimento deste projecto aparenta ser a ausência de documentação adequada.
