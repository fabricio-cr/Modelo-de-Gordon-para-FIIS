# Modelo de Gordon para FIIs

O modelo de Gordon é utilizado para precificar o valor financeiro de uma ação, mas também é frequentemente utilizado para o estabelecimento de valor de outras espécies de ativos. Eles se encaixam perfeitamente na precificação de Fundos de Investimento Imobiliários e é, frequentemente, utilizado por muitos gestores. Tal modelo se baseia na estimativa de dividendos futuros que crescem a taxas constantes e, por conta disso, é preciso que se tenha muita sensatez ao utilizá-lo pois, como se sabe, os dividendos, assim como as demais métricas e características das empresas, dificilmente seguem o mesmo padrão no longo prazo. 

A precificação do ativo gerada pelo modelo é baseada na seguinte fórmula matemática: 

<p align="center">
  <img src="https://www.suno.com.br/wp-content/uploads/2017/10/MODELO-GORDON.jpg" width="350" title="hover text">
</p>

Para mais informações sobre o modelo veja https://youtu.be/7oplNshpLBI.

Neste simples projeto, ao escolher uma lista de FIIs, gera-se um Data Frame com os últimos dividendos pagos pelo fundo e um dicionário com a soma dos últimos 12 dividendos a fim fornecer uma base para o investidor definir o valor D. Ademais, gera-se um Data Frame com taxas atualizadas do tesouro direto e um Data Frame com a expectativa do mercado para o IPCA nos próximos 12 meses onde o mesmo é proveniente do Banco Central. Estas informações ajudam o investidor a escolher uma boa taxa de desconto K para o modelo em questão. Por fim, gera-se um Data Frame com valores atuais dos FIIs escolhidos e valores gerados pelo Modelo. Todas as informações mencionadas são atualizadas diariamente pelas fontes inseridas no script.
