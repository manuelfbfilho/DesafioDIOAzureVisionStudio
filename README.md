<h1>
    <a href="https://www.dio.me/">
     <img align="center" width="40px" src="https://hermes.digitalinnovation.one/assets/diome/logo-minimized.png"></a>
    <span> Desafio Azure AI Vision Studio | Read text in Vision Studio</span>
</h1>

Repositório criado como atividade para avaliação parcial do treinamento para realizar a prova de certificação no Microsoft Azure AI Fundamentals (AI Fundamentals +AI-900) da [Digital Innovation One](https://www.dio.me/).

Será utilizado o serviço de IA do Azure para explorar os recursos de reconhecimento óptico de caracteres do Azure AI Vision. Usarei o Vision Studio para experimentar extrair texto de imagens, sem precisar escrever nenhum código.

Um desafio comum de visão computacional é detectar e interpretar texto incorporado em uma imagem. Isso é conhecido como reconhecimento óptico de caracteres (OCR). Aqui usarei um recurso de serviços de IA do Azure, que inclui os serviços de Visão de IA do Azure. Em seguida, usarei o Vision Studio para experimentar o OCR com diferentes tipos de imagens.

## Objetivo 🎯
Conhecer o Azure Vision Studio e aprender a utilizar a plataforma e unir o conhecimento teórico com a prática.


## Passo-a-Passo 🛠️

### 1. Crie um novo repositório no GitHub
   * 1.1 Acesse o seu repositório no GitHub.
   * 1.2 Clique no botão “Add file” e selecione “Create new file”.
   * 1.3 Digite “inputs/” na caixa de texto (incluindo a barra no final).
   * 1.4 Em seguida, dê um nome para o arquivo (por exemplo, “placeholder.txt”) e faça o commit.<br>
     <b>Ps.:</b> Para a criação da psta "outputs" siga os mesmos passos acima, substituindo "inputs" por "outputs".


### 2. Criar um recurso de serviços de IA do Azure
Você pode usar os recursos de OCR do Azure AI Vision com um recurso multisserviço dos serviços de IA do Azure. Se você ainda não tiver feito isso, crie um recurso de serviços de IA do Azure em sua assinatura do Azure.

2.1	Em outra guia do navegador, abra o portal do Azure em https://portal.azure.com, entrando com a conta da Microsoft associada à sua assinatura do Azure.

2.2	Clique no botão +Criar um recurso e procure serviços de IA do Azure. Selecione criar um plano de serviços de IA do Azure. Você será levado a uma página para criar um recurso de serviços de IA do Azure. Configure-o com as seguintes configurações:<br>
&nbsp;&nbsp;&nbsp;o	Assinatura: sua assinatura do Azure.<br>
&nbsp;&nbsp;&nbsp;o	Grupo de recursos: selecione ou crie um grupo de recursos com um nome exclusivo.<br>
&nbsp;&nbsp;&nbsp;o	Região: Leste dos EUA (East US).<br>
&nbsp;&nbsp;&nbsp;o	Nome: insira um nome exclusivo.<br>
&nbsp;&nbsp;&nbsp;o	Nível de preços: Standard S0.<br>
&nbsp;&nbsp;&nbsp;o	Ao marcar esta caixa, reconheço que li e entendi todos os termos abaixo: Selecionado.
  
2.3	Selecione Revisar + criar e, em seguida, Criar e aguarde a conclusão da implantação.
<br>

### 3. Conectar seu recurso de serviço de IA do Azure ao Vision Studio
3.1	Em outra guia do navegador, navegue até o Vision Studio em [Azure Vision Studio](https://portal.vision.cognitive.azure.com).<br>
3.2	Entre com sua conta e verifique se você está usando o mesmo diretório em que criou seu recurso de serviços de IA do Azure.
3.3 Na home page do Vision Studio, selecione Exibir todos os recursos no cabeçalho Introdução ao Vision.
![image](https://github.com/manuelfbfilho/DesafioDIOAzureVisionStudio/assets/151965418/f1fafd3f-80d6-4a36-8815-281c4ae0fcb2)

3.4 Na página Selecione um recurso para trabalhar, passe o cursor do mouse sobre o recurso criado acima na lista e marque a caixa à esquerda do nome do recurso e selecione Selecionar como recurso padrão. Se o recurso não estiver listado, talvez seja necessário atualizar a página.
![image](https://github.com/manuelfbfilho/DesafioDIOAzureVisionStudio/assets/151965418/eb6999df-9d4d-445a-851e-3e506f154a65)

3.5 Feche a página de configurações selecionando o "x" no canto superior direito da tela.
<br><br>
### 4. Extrair texto de imagens no Vision Studio
4.1	Em um navegador da Web, navegue até o Vision Studio em [Azure Vision Studio](https://portal.vision.cognitive.azure.com).<br>
4.2 Na página inicial Introdução ao Vision, selecione Reconhecimento óptico de caracteres e o bloco Extrair texto de imagens.<br>
4.3 No subtítulo Experimentar, reconheça a política de uso de recursos lendo e marcando a caixa.<br>
4.4 Selecione (https://aka.ms/mslearn-ocr-images) para baixar ocr-images.zip. Em seguida, abra a pasta.<br>
4.5 No portal, selecione Procurar um arquivo e navegue até a pasta no computador em que você baixou ocr-images.zip. Selecione advert.jpg e selecione Abrir.<br>
4.6 Agora reveja o que é devolvido:<br>
o	Em Atributos detectados, qualquer texto encontrado na imagem é organizado em uma estrutura hierárquica de regiões, linhas e palavras.<br>
o	Na imagem, a localização do texto é indicada por uma caixa delimitadora, como mostrado aqui:
![image](https://github.com/manuelfbfilho/DesafioDIOAzureVisionStudio/assets/151965418/fa7495ed-5fb5-413e-9845-fe025e51520d)
<br>
4.7 Agora você pode tentar outra imagem. Selecione Procurar um arquivo e navegue até a pasta onde você salvou os arquivos do GitHub. Selecione carta.jpg.
![image](https://github.com/manuelfbfilho/DesafioDIOAzureVisionStudio/assets/151965418/db6e3dbe-64cf-47a6-a1c4-ea61065a7da8)
<br>
4.8 8.	Analise os resultados da segunda imagem. Ele deve retornar o texto e as caixas delimitadoras do texto. Se tiver tempo, tente note.jpg e receipt.jpg.
<br>
#### Parabéns! Você fez todo o processo!

### ATENÇÃO Após Terminar todo o Processo
Se você não pretende fazer mais exercícios, exclua todos os recursos que não são mais necessários. Isso evita o acúmulo de custos desnecessários.
1.	Abra o portal do Azure em https://portal.azure.com e selecione o grupo de recursos que contém o recurso que você criou.
2.	Selecione o recurso e selecione Excluir e, em seguida, Sim para confirmar. O recurso é excluído.

---
##  Desafio: Profile README

### Como Entregar esse projeto?
Chegou a hora de você construir um portfólio ainda mais rico e impressionar futuros recrutadores, para isso é sempre importante mostrar os resultados do seu esforço e como você os obteve deixando claro o seu racional, para isso faça da seguinte maneira: 😊💙.

1. Crie um novo repositório no github com um nome a sua preferência
2. Crie uma pasta chamada 'inputs' e salve as imagens que você utilizou
3. Crie uma pasta chamado 'output' e salve os resultados de reconhecimento de texto nessas imagens
4. Crie um arquivo chamado readme.md , deixe alguns prints descreva o processo, alguns insights e possibilidades que você aprendeu durante o conteúdo.
5. Compartilhe conosco o link desse repositório através do botão 'entregar projeto'
---

## Contatos 
[![Linkedin](https://img.shields.io/badge/Linkedin-000?style=for-the-badge&logo=linkedin&logoColor=30A3DC)](https://www.linkedin.com/in/manuelfbfilho)
<br>
[![GitHub](https://img.shields.io/badge/GitHub-000?style=for-the-badge&logo=github&logoColor=30A3DC)](https://github.com/manuelfbfilho)

