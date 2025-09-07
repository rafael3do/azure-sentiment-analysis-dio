Exercício – Estudo de sentimentos com Language Studio no Azure AI

A funcionalidade análise de sentimentos e opiniões disponível no Language Studio, da Azure, possibilita identificar emoções positivas, negativas ou neutras em diferentes textos. Este repositório apresenta exemplos de experimentos feitos na plataforma. As atividades foram realizadas durante o Bootcamp Microsoft Azure AI Fundamentals, da DIO.

Índice

Etapas do processo

Resultados obtidos

Reflexões e conclusão

Etapas do processo

Os testes seguiram as orientações do Microsoft Learn. Para detalhes adicionais, consulte a página Analyze text with Language Studio
.

Criando um recurso do Azure Language Service

Para utilizar o Language Studio é necessário primeiro vincular um recurso do Language Service à sua conta Azure. O procedimento é o seguinte:

Acessar portal.azure.com
.

Criar um novo recurso Language Service através da opção Create Resource.

<div align="center"> <img src="readmeFiles/01.png" alt="Create a resource" width="600"/> 
</div> <div align="center"> <img src="readmeFiles/03.png" alt="Create a resource" width="600"/> </div>

Aguardar a conclusão da implantação do recurso.

Conectando o recurso ao Language Studio

Com o recurso criado, é necessário associá-lo ao Language Studio. Para isso:

Acesse o Language Studio
.

Na tela inicial, selecione a opção Select a resource para visualizar os serviços criados.

<div align="center"> <img src="readmeFiles/04.png" alt="View all resources" width="800"/> </div>

Insira as informações solicitadas e selecione o recurso recém-configurado.

<div align="center"> <img src="readmeFiles/05.png" alt="Set default resource" width="800"/> </div>
Escolhendo e testando o serviço

Após concluir a configuração, a tela inicial exibe os recursos disponíveis para uso. Neste estudo foi selecionada a opção Analyze sentiment and mine opinions, localizada na aba Classify text.

<div align="center"> <img src="readmeFiles/06.png" alt="Language Studio Services" width="800"/> </div>
Resultados obtidos

No serviço é possível inserir o texto que será avaliado, escolher o idioma e ativar a opção de análise de opiniões.

<div align="center"> <img src="readmeFiles/07.png" alt="Language Studio Services" width="800"/> </div>

O resultado da análise indicou que o texto possuía predominância de sentimento negativo (65%), embora a confiança do modelo fosse apenas 25%. Interessante observar que algumas frases foram classificadas com alta taxa de confiança, enquanto outras receberam marcação de 100% negativo, mas com 0% de confiança.

<div align="center"> <img src="readmeFiles/08.png" alt="Language Studio Services" width="400"/> </div> <br>
Reflexões e conclusão

Recursos de identificação de sentimentos podem auxiliar bastante na análise automática de comentários e avaliações de serviços ou produtos. O desempenho tende a ser melhor quando os textos realmente transmitem opiniões claras. Entretanto, quando a intenção não é explícita, os resultados podem não ser tão precisos.

Isso provavelmente ocorre porque a ferramenta interpreta frases de forma isolada, sem considerar o contexto geral do texto. Uma solução capaz de relacionar sentenças e interpretar o conjunto como um todo poderia alcançar resultados mais consistentes.