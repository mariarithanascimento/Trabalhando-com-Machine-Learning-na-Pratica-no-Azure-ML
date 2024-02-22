# Trabalhando com Machine Learning na Prática no Azure ML

## Crie um espaço de trabalho do Azure Machine Learning

Para utilizar o Azure Machine Learning, é necessário aprovisionar um **espaço de trabalho** do Azure Machine Learning na sua subscrição do Azure. Depois, você poderá usar o estúdio Azure Machine Learning para trabalhar com os recursos do seu workspace.

<aside>
💡 Dica : se você já tiver um espaço de trabalho do Azure Machine Learning, poderá usá-lo e pular para a próxima tarefa.

</aside>

Entre no [portal](https://portal.azure.com/) do Azure usando  suas credenciais da Microsoft.

**Selecione + Criar um recurso** , pesquise **Machine Learning** e crie um novo recurso do Azure Machine Learning com as seguintes configurações:

***Assinatura:** sua assinatura do Azure .
**Grupo de recursos:** Crie ou selecione um grupo de recursos .
**Nome:** Insira um nome exclusivo para seu espaço de trabalho .
**Região:** Selecione a região geográfica mais próxima .
**Conta de armazenamento:** observe a nova conta de armazenamento padrão que será criada para seu espaço de trabalho .
**Cofre de chaves:** Observe o novo cofre de chaves padrão que será criado para seu espaço de trabalho.
**Insights de aplicativo:** observe o novo recurso padrão de insights de aplicativo que será criado para seu espaço de trabalho .
**Registro de contêiner:** Nenhum ( um será criado automaticamente na primeira vez que você implantar um modelo em um contêiner ).*

Selecione Revisar + criar e selecione Criar . Aguarde a criação do seu espaço de trabalho (pode demorar alguns minutos) e, em seguida, vá para o recurso implantado.

Selecione Launch Studio (ou abra uma nova guia do navegador e navegue até [https://ml.azure.com](https://ml.azure.com/) e entre no Azure Machine Learning Studio usando sua conta da Microsoft). Feche todas as mensagens exibidas.

No estúdio Azure Machine Learning, você deverá ver seu espaço de trabalho recém-criado. Caso contrário, selecione Todos os espaços de trabalho no menu à esquerda e selecione o espaço de trabalho que você acabou de criar.

<aside>
📌 Para seguir para o próximo passo, deve seguir o passo a passo do tutorial [Criar um trabalho de Azure Machine Learning automatizado](https://learn.microsoft.com/pt-br/azure/machine-learning/tutorial-first-experiment-automated-ml?view=azureml-api-2#create-an-automated-machine-learning-job)

</aside>

Na página inicial do seu Workspace, clique em **ML automatizado**

![Untitled](Trabalhando%20com%20Machine%20Learning%20na%20Pra%CC%81tica%20no%20Az%20354904732fb949a9811fea398d62efed/Untitled.png)

Selecione qual trabalho deseja utilizar, nesse caso usaremos o “mslearn-bike-automl”

![Untitled](Trabalhando%20com%20Machine%20Learning%20na%20Pra%CC%81tica%20no%20Az%20354904732fb949a9811fea398d62efed/Untitled%201.png)

Ao abrir a página, clique na guia **Modelos + trabalhos filho** e selecione um modelo de sua preferência

![Untitled](Trabalhando%20com%20Machine%20Learning%20na%20Pra%CC%81tica%20no%20Az%20354904732fb949a9811fea398d62efed/Untitled%202.png)

Clique em **Implantar** e selecione **Serviços Web**

![Untitled](Trabalhando%20com%20Machine%20Learning%20na%20Pra%CC%81tica%20no%20Az%20354904732fb949a9811fea398d62efed/Untitled%203.png)

A tela seguinte deve ser preenchida com as seguintes configurações:

- ***Nome**: prever-aluguéis*
- ***Descrição**: Prever aluguel de bicicletas*
- ***Tipo de computação**: Instância de Contêiner do Azure*
- ***Habilitar autenticação:** selecionado*

> Implantar

![Untitled](Trabalhando%20com%20Machine%20Learning%20na%20Pra%CC%81tica%20no%20Az%20354904732fb949a9811fea398d62efed/Untitled%204.png)

Assim que o modelo ser implantado > pontos de extremidade > prever-alugueis

![Untitled](Trabalhando%20com%20Machine%20Learning%20na%20Pra%CC%81tica%20no%20Az%20354904732fb949a9811fea398d62efed/Untitled%205.png)

Nessa tela ainda podemos: Testa-lo, consumi-lo e verificar seus logs

![Untitled](Trabalhando%20com%20Machine%20Learning%20na%20Pra%CC%81tica%20no%20Az%20354904732fb949a9811fea398d62efed/Untitled%206.png)
