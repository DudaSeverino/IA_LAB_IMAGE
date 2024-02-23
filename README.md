# IA_LAB_IMAGE
# Tutorial.

Criar um recurso de serviços de **IA do Azure** Você pode usar os recursos de análise de imagem do Azure AI Vision com um recurso multisserviço dos **serviços de IA do Azure**. Se você ainda não tiver feito isso, crie um recurso de serviços de IA do Azure em sua assinatura do Azure.

1. Em outra guia do navegador, abra o portal do Azure em  [https://portal.azure.com](https://portal.azure.com/), entrando com a conta da Microsoft associada à sua assinatura do Azure.

2. Clique no botão +Criar um recurso e procure serviços de IA do Azure. Selecione criar um plano de serviços de IA do Azure. Você será levado a uma página para criar um recurso de serviços de IA do Azure. Configure-o com as seguintes configurações: 
   **Assinatura**: sua assinatura do Azure. Grupo de recursos: selecione ou crie um grupo de recursos com um nome exclusivo. 
  ** Região**: Leste dos EUA. 
   **Nome**: insira um nome exclusivo. 
   **Nível de preços**: Standard S0.
   **Ao marcar esta caixa, reconheço que li e entendi todos os termos abaixo**: Selecionado. 

3. Selecione Revisar + criar e, em seguida, Criar e aguarde a conclusão da implantação.


# Conectar seu recurso de serviço de IA do Azure ao Vision Studio 
Em seguida, conecte o recurso de serviço de IA do Azure provisionado acima ao Vision Studio.

1. Em outra guia do navegador, navegue até o Vision Studio.

2. Entre com sua conta e verifique se você está usando o mesmo diretório em que criou seu recurso de serviços de IA do Azure.

3. Na home page do Vision Studio, selecione Exibir todos os recursos no cabeçalho Introdução ao Vision.

O link Exibir todos os recursos está realçado em Introdução ao Vision no Vision Studio.

4. Na página Selecione um recurso para trabalhar, passe o cursor do mouse sobre o recurso criado acima na lista e marque a caixa à esquerda do nome do recurso e selecione **Selecionar como recurso padrão.**

5. Feche a página de configurações selecionando o "x" no canto superior direito da tela.

# Gerar legendas para uma imagem 
Agora você está pronto para usar o Vision Studio para analisar imagens tiradas por uma câmera na loja Northwind Traders.

Vejamos a funcionalidade de legendagem de imagem do Azure AI Vision. As legendas de imagem estão disponíveis por meio dos recursos Legenda e Legendas densas.

1 .Em um navegador da Web, navegue até o Vision Studio.

2. Na página inicial Introdução ao Vision, selecione a guia Análise de imagem e selecione o bloco Adicionar legendas a imagens.

3. No subtítulo Experimentar, reconheça a política de uso de recursos lendo e marcando a caixa.

4. Selecione  [https://aka.ms/mslearn-images-for-analysis](https://aka.ms/mslearn-images-for-analysis)  para baixar image-analysis.zip. Abra a pasta em seu computador e localize o arquivo chamado store-camera-1.jpg; que contém a seguinte imagem:

5. Carregue a imagem store-camera-1.jpg arrastando-a para a caixa Arrastar e soltar arquivos aqui ou navegando até ela em seu sistema de arquivos.

6. Observe o texto da legenda gerado, visível no painel Atributos detectados à direita da imagem.

7. Em seguida, use a mesma imagem para executar legendas densas. Retorne à home page do Vision Studio e, como fez antes, selecione a guia Análise de imagem e, em seguida, selecione o bloco Legenda densa.

O recurso Legendas densas difere do recurso Legenda porque fornece várias legendas legíveis por humanos para uma imagem, uma descrevendo o conteúdo da imagem e outras, cada uma cobrindo os objetos essenciais detectados na imagem. Cada objeto detectado inclui uma caixa delimitadora, que define as coordenadas de pixel dentro da imagem associada ao objeto.

 8. Passe o mouse sobre uma das legendas na lista Atributos detectados e observe o que acontece na imagem.

Mova o cursor do mouse sobre as outras legendas da lista e observe como a caixa delimitadora muda na imagem para realçar a parte da imagem usada para gerar a legenda.

# Marcação de imagens 

O próximo recurso que você tentará é a funcionalidade Extrair tags. As tags de extração são baseadas em milhares de objetos reconhecíveis, incluindo seres vivos, cenários e ações.

1. Retorne à home page do Vision Studio e selecione o bloco Extrair marcas comuns de imagens na guia Análise de imagem.

2.  Em Escolha o modelo que você deseja experimentar, deixe Produto pré-criado versus modelo de intervalo selecionado. Em Escolha seu idioma, selecione Inglês ou um idioma de sua preferência.

3. Abra a pasta que contém as imagens que você baixou e localize o arquivo chamado store-image-2.jpg, que tem a seguinte aparência:

4. Carregue o arquivo store-camera-2.jpg.

5. Revise a lista de tags extraídas da imagem e a pontuação de confiança para cada uma no painel de atributos detectados. Aqui, o escore de confiança é a probabilidade de que o texto para o atributo detectado descreva o que realmente está na imagem. Observe na lista de tags que ela inclui não apenas objetos, mas ações, como comprar, vender e ficar em pé.

# Detecção de objetos 
Nesta tarefa, você usa o recurso de detecção de objeto da análise de imagem. A detecção de objetos detecta e extrai caixas delimitadoras com base em milhares de objetos reconhecíveis e seres vivos.

1. Retorne à home page do Vision Studio e selecione o bloco Detectar objetos comuns em imagens na guia Análise de imagem.

2. Em Escolha o modelo que você deseja experimentar, deixe Produto pré-criado versus modelo de intervalo selecionado.

3. Abra a pasta que contém as imagens que você baixou e localize o arquivo chamado store-camera-3.jpg, que tem a seguinte aparência:

4. Carregue o arquivo store-camera-3.jpg.

5. Na caixa Atributos detectados, observe a lista de objetos detectados e suas pontuações de confiança.

6. Passe o cursor do mouse sobre os objetos na lista Atributos detectados para realçar a caixa delimitadora do objeto na imagem.

7. Mova o controle deslizante Valor de limite até que um valor de 70 seja exibido à direita do controle deslizante. Observe o que acontece com os objetos na lista. O controle deslizante de limite especifica que somente objetos identificados com uma pontuação de confiança ou probabilidade maior que o limite devem ser exibidos.

# Arrumar
 Se você não pretende fazer mais exercícios, exclua todos os recursos que não são mais necessários. Isso evita o acúmulo de custos desnecessários.

1. Abra o portal do Azure e selecione o grupo de recursos que contém o recurso que você criou. 
2. Selecione o recurso e selecione Excluir e, em seguida, Sim para confirmar. 

O recurso é excluído

![image](https://github.com/DudaSeverino/IA_LAB_IMAGE/assets/125839474/598ff1aa-9462-4577-b2a3-7ef99b452a99)

