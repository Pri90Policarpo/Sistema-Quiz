{

"registros": {

"1": {

"type": "quiz", 

"text": "Your company has decided to make a major revision of their API in order to create better experiences for their developers. They need to keep the old version of the API available and deployable, while allowing new customers and testers to try out the new API. They want to keep the same SSL and DNS records in place to serve both APIs.\nWhat should they do?", <!--***(Sua empresa decidiu fazer uma grande revisão em sua API para criar melhores experiências para seus desenvolvedores. Eles precisam manter a versão  antiga da API disponivel e implantável, enquanto permitem que novos clientes e testadores experimentem a nova API. Eles querem manter os mesmos registros SSL e DNS para servir ambas APIs. O que eles devem fazer? )***-->

"options": [

{

"text": "A. Configure a new load balancer for the new version of the API", ***<!--(Configure um novo balanceador de carga para a nova versão da API)-->***

"explanation": "Configuring a new load balancer would require separate SSL and DNS records for each load balancer, which contradicts the requirement to keep the same SSL and DNS records.", ***<!--(Configurar um novo balanceador de carga exigiria registros SSL e DNS separados para cada balanceador de carga, o que contradiz o requisito de manter os mesmos registros SSL e DNS.)-->***

"correct": false

}, 

{

"text": "B. Reconfigure old clients to use a new endpoint for the new API", ***<!--(Reconfigure clientes antigos para usar um novo endpoint para a nova API")-->***

"explanation": "Reconfiguring old clients to use a new endpoint would disrupt existing clients and negate the need to keep the same SSL and DNS records.", ***<!--("Reconfigurar clientes antigos para usar um novo endpoint interromperia os clientes existentes e eliminaria a necessidade de manter os mesmos registros SSL e DNS.",)-->***

"correct": false

}, 

{

"text": "C. Have the old API forward traffic to the new API based on the path", ***<!--(Faça com que a API antiga encaminhe o tráfego para a nova API com base no caminho",)-->***

"explanation": "This approach involves adding unnecessary complexity to the old API, and it does not leverage the capabilities of load balancers to manage traffic efficiently between different API versions.", ***<!--("Essa abordagem envolve adicionar complexidade desnecessária à API antiga e não aproveita os recursos dos balanceadores de carga para gerenciar o tráfego de forma eficiente entre diferentes versões da API.",)-->***

"correct": false

},

 {

"text": "D. Use separate backend pools for each API path behind the load balancer", ***<!--(Use pools de back-end separados para cada caminho de API por trás do balanceador de carga",)-->***

"explanation": "This is the best solution as it allows the load balancer to route traffic to the appropriate backend pool based on the API path. This method keeps the same SSL and DNS records while enabling both versions of the API to be served from the same endpoint. It also provides a clean separation of concerns, allowing each API version to be managed independently.", ***<!--("Esta é a melhor solução, pois permite que o balanceador de carga direcione o tráfego para o pool de back-end apropriado com base no caminho da API. Este método mantém os mesmos registros SSL e DNS enquanto permite que ambas as versões da API sejam atendidas no mesmo endpoint. Ele também fornece uma separação clara de interesses, permitindo que cada versão da API seja gerenciada de forma independente.",)-->***

"correct": true

}

]

},

"2": {

"type": "quiz", 

"text": "Your company plans to migrate a multi-petabyte data set to the cloud. The data set must be available 24hrs a day. Your business analysts have experience only with using a SQL interface.\nHow should you store the data to optimize it for ease of analysis?", "options": [ (***<!--"Sua empresa planeja migrar um conjunto de dados de vários petabytes para a nuvem. O conjunto de dados deve estar disponível 24 horas por dia. Seus analistas de negócios têm experiência apenas no uso de uma interface SQL.\nComo você deve armazenar os dados para otimizá-los para facilitar de análise?", "opções")-->***

{

"text": "A. Load data into Google BigQuery", ***<!--(Carregar dados no Google BigQuery",)-->***

"explanation": " Google BigQuery is a fully managed, serverless, highly scalable data warehouse that supports SQL queries. It is designed for analyzing large datasets quickly and efficiently. BigQuery can handle multi-petabyte datasets and offers 24/7 availability. It is optimized for ease of analysis with its support for standard SQL, which aligns perfectly with the business analysts' experience.", *<!--**(O Google BigQuery é um data warehouse totalmente gerenciado, sem servidor e altamente escalonável que oferece suporte a consultas SQL. Ele foi projetado para analisar grandes conjuntos de dados de forma rápida e eficiente. O BigQuery pode lidar com conjuntos de dados de vários petabytes e oferece disponibilidade 24 horas por dia, 7 dias por semana. Ele é otimizado para facilitar o gerenciamento análise com suporte para SQL padrão, que se alinha perfeitamente com a experiência dos analistas de negócios.")**-->*

"correct": true

}, 

{

"text": "B. Insert data into Google Cloud SQL", ***<!--(Insira dados no Google Cloud SQL",)-->***

"explanation": "Google Cloud SQL is a managed relational database service that supports SQL, but it is not designed to handle multi-petabyte datasets efficiently. It is more suitable for smaller-scale applications and workloads. For extremely large datasets, performance and scalability would be significant concerns.", ***<!--("O Google Cloud SQL é um serviço de banco de dados relacional gerenciado que oferece suporte a SQL, mas não foi projetado para lidar com conjuntos de dados de vários petabytes de maneira eficiente. É mais adequado para aplicativos e cargas de trabalho de menor escala. Para conjuntos de dados extremamente grandes, o desempenho e a escalabilidade seriam significativos preocupações.")-->***

"correct": false

},

{

"text": "C. Put flat files into Google Cloud Storage", ***<!--(Coloque arquivos simples no Google Cloud Storage",)-->***

"explanation": "Google Cloud Storage is an object storage service ideal for storing large amounts of unstructured data, such as flat files. While it can store multi-petabyte datasets and offers high availability, it is not optimized for SQL-based analysis. To analyze the data, you would need to load it into a service like BigQuery or a similar database, adding an extra step.", ***<!--("O Google Cloud Storage é um serviço de armazenamento de objetos ideal para armazenar grandes quantidades de dados não estruturados, como arquivos simples. Embora possa armazenar conjuntos de dados de vários petabytes e ofereça alta disponibilidade, não é otimizado para análise baseada em SQL. Para analisar os dados , você precisaria carregá-lo em um serviço como o BigQuery ou um banco de dados semelhante, adicionando uma etapa extra.",)-->***

"correct": false

},

{

"text": "D. Stream data into Google Cloud Datastore", **<!--(Transmitir dados para o Google Cloud Datastore)-->**

"explanation": "Google Cloud Datastore is a NoSQL document database designed for web and mobile applications. It does not natively support SQL queries and is not optimized for multi-petabyte datasets or traditional analytical workloads. Using Datastore would complicate the analysis process for business analysts accustomed to SQL.", ***<!--("O Google Cloud Datastore é um banco de dados de documentos NoSQL projetado para aplicativos da Web e móveis. Ele não oferece suporte nativo a consultas SQL e não é otimizado para conjuntos de dados de vários petabytes ou cargas de trabalho analíticas tradicionais. Usar o Datastore complicaria o processo de análise para analistas de negócios acostumados com SQL )-->***

"correct": false

}

]

},

"3": {

"type": "quiz", 

"text": "The operations manager asks you for a list of recommended practices that she should consider when migrating a J2EE application to the cloud.\nWhich three practices should you recommend? (Choose three.)\n",  ***<!--("A gerente de operações pede uma lista de práticas recomendadas que ela deve considerar ao migrar um aplicativo J2EE para a nuvem.\nQuais três práticas você deve recomendar? (Escolha três.)\n",)-->***

"options": [

{

"text": "A. Port the application code to run on Google App Engine", "explanation": "Google App Engine is a fully managed serverless platform that allows you to deploy and run applications without managing the underlying infrastructure. Migrating a J2EE application to App Engine can take advantage of its scalability, load balancing, and integrated development environment.",  <!--***(Portar o código do aplicativo para execução no Google App Engine", "explanation": "O Google App Engine é uma plataforma sem servidor totalmente gerenciada que permite implantar e executar aplicativos sem gerenciar a infraestrutura subjacente. A migração de um aplicativo J2EE para o App Engine pode aproveitar a escalabilidade, o balanceamento de carga e o ambiente de desenvolvimento integrado.",)***-->

"correct": true

},

{

"text": "B. Integrate Cloud Dataflow into the application to capture real-time metrics", <!--(Integre o Cloud Dataflow ao aplicativo para capturar métricas em tempo real",)-->

"explanation": "Cloud Dataflow is primarily used for stream and batch data processing. While it is a powerful tool for real-time data analytics, it is not directly relevant to the migration of a J2EE application to the cloud. Capturing real-time metrics is important, but there are more suitable tools for application monitoring and logging, such as Stackdriver (now part of Google Cloud's Operations suite).", <!--"explanation": "O Cloud Dataflow é usado principalmente para processamento de dados em fluxo e em lote. Embora seja uma ferramenta poderosa para análise de dados em tempo real, não é diretamente relevante para a migração de um aplicativo J2EE para a nuvem. Captura em tempo real métricas são importantes, mas existem ferramentas mais adequadas para monitoramento e registro de aplicativos, como o Stackdriver (agora parte do pacote de operações do Google Cloud).",-->

"correct": false

},

{

"text": "C. Instrument the application with a monitoring tool like Stackdriver Debugger", (<!--Instrumente o aplicativo com uma ferramenta de monitoramento como o Stackdriver Debugger")-->

"explanation": "Monitoring tools are essential for tracking the performance, availability, and reliability of applications in the cloud. Stackdriver Debugger (now part of Google Cloud's Operations suite) provides real-time insights into the application\u2019s behavior, which is crucial for managing and optimizing the application post-migration.", <!--("As ferramentas de monitoramento são essenciais para monitorar o desempenho, a disponibilidade e a confiabilidade dos aplicativos na nuvem. O Stackdriver Debugger (agora parte do pacote Operations do Google Cloud) fornece insights em tempo real sobre o comportamento do aplicativo, o que é crucial para gerenciar e otimizar a aplicação pós-migração.",)-->

"correct": true

},

{

"text": "D. Select an automation framework to reliably provision the cloud infrastructure", <!-- Selecione uma estrutura de automação para provisionar de forma confiável a infraestrutura em nuvem" -->

"explanation": "Using an automation framework (like Terraform or Google Deployment Manager) ensures that the cloud infrastructure is provisioned reliably and consistently. Automation helps reduce human error, improves repeatability, and allows for version control of infrastructure configurations.",   <!--"O uso de uma estrutura de automação (como Terraform ou Google Deployment Manager) garante que a infraestrutura em nuvem seja provisionada de maneira confiável e consistente. A automação ajuda a reduzir erros humanos, melhora a repetibilidade e permite o controle de versão das configurações de infraestrutura.",-->

"correct": true

},

{

"text": "E. Deploy a continuous integration tool with automated testing in a staging environment", "explanation": "While continuous integration and automated testing are best practices for software development and deployment, they are not specific to the migration of a J2EE application to the cloud. This practice is more about the ongoing development process rather than the migration itself.", <!--Implante uma ferramenta de integração contínua com testes automatizados em um ambiente de teste", "explicação": "Embora a integração contínua e os testes automatizados sejam práticas recomendadas para desenvolvimento e implantação de software, eles não são específicos para a migração de um aplicativo J2EE para a nuvem. Esta prática tem mais a ver com o processo de desenvolvimento contínuo do que com a migração em si."-->

"correct": false

}, 

{

"text": "F. Migrate from MySQL to a managed NoSQL database like Google Cloud Datastore or Bigtable", <!--Migre do MySQL para um banco de dados NoSQL gerenciado como Google Cloud Datastore ou Bigtable-->

"explanation": "Migrating from MySQL to a managed NoSQL database is a significant architectural change and may not be necessary or appropriate for a J2EE application. The choice of database should be based on the specific needs of the application. If the application is already using a relational database, it might be more straightforward to migrate to a managed relational database service like Google Cloud SQL.",   <!--"Migrar do MySQL para um banco de dados NoSQL gerenciado é uma mudança arquitetural significativa e pode não ser necessária ou apropriada para uma aplicação J2EE. A escolha do banco de dados deve ser baseada nas necessidades específicas da aplicação. Se a aplicação já estiver usando um banco de dados relacional , pode ser mais simples migrar para um serviço de banco de dados relacional gerenciado como o Google Cloud SQL.",-->

"correct": false

}

]

},

"4": {

"type": "quiz", 

"text": "A news feed web service has the following code running on Google App Engine. During peak load, users report that they can see news articles they already viewed.\nWhat is the most likely cause of this problem?\n\n```\nimport news\nfrom flask import Flask, redirect, request \nfrom flask.ext.api import status \nfrom google.appengine.api import users\n\napp = Flask (_name_)\ngessiong = ()\n\n@app. route (\"/\") def homepage () :\n\t\t\t\tuser = users.get_current_user ()\n\t\t\t\tif not user:\n\t\t\t\t\t\t\t\treturn \"Invalid login\", status.HTTP_401_UNAUTHORIZED\n\t\t\t\tif user not in sessions:\n\t\t\t\t\t\t\t\tsessions (user] = {\"viewed\": []}|\n\t\t\t\t\n\t\t\t\tnews_articles = news.get_new_news (user, sessions [user][\"viewed\" ])\n\t\t\t\tsessions (user] [\"viewed\"] +- In[\"id\"] for n in news_articles\uff3d\n\n\t\t\t\treturn news. render (news_articles)\n\nif __name__ == \"_main\":\n\t\t\t\tapp.run()\n```",   <!--"Um serviço da Web de feed de notícias tem o seguinte código em execução no Google App Engine. Durante o pico de carga, os usuários relatam que podem ver artigos de notícias que já visualizaram.\nQual é a causa mais provável desse problema?-->

"options": [

{

"text": "A. The session variable is local to just a single instance Most Voted",   <!--A variável de sessão é local para apenas uma única instância Mais Votada",-->

"explanation": "This is the correct answer because it directly addresses the issue of sessions being local to each instance and not shared across instances, leading to the observed problem.",  <!--"Esta é a resposta correta porque aborda diretamente a questão das sessões serem locais para cada instância e não compartilhadas entre instâncias, levando ao problema observado.",-->



"correct": true

},

{

"text": "B. The session variable is being overwritten in Cloud Datastore",   <!--A variável de sessão está sendo substituída no Cloud Datastore",-->

"explanation": "This is incorrect because the code does not use Cloud Datastore for storing session information.",   <!--"Isso está incorreto porque o código não usa o Cloud Datastore para armazenar informações da sessão.",-->

"correct": false

}, 

{

"text": "C. The URL of the API needs to be modified to prevent caching",   <!--A URL da API precisa ser modificada para evitar o armazenamento em cache",-->

"explanation": "This is incorrect because the issue is related to session handling, not caching of API responses.",  <!--"Isso está incorreto porque o problema está relacionado ao tratamento da sessão, não ao cache das respostas da API.",-->

"correct": false

},

{

"text": "D. The HTTP Expires header needs to be set to -1 stop caching",   <!--O cabeçalho HTTP Expires precisa ser definido como -1 stop caching",-->

"explanation": " This is incorrect because the issue is related to session management, not HTTP caching headers.",  <!--"Isso está incorreto porque o problema está relacionado ao gerenciamento de sessão, não aos cabeçalhos de cache HTTP.",-->

"correct": false

}

]

},

"5": {

"type": "quiz", 

"text": "An application development team believes their current logging tool will not meet their needs for their new cloud-based product. They want a better tool to capture errors and help them analyze their historical log data. You want to help them find a solution that meets their needs.\nWhat should you do?",   <!--"Uma equipe de desenvolvimento de aplicativos acredita que sua ferramenta de registro atual não atenderá às necessidades de seu novo produto baseado em nuvem. Eles querem uma ferramenta melhor para capturar erros e ajudá-los a analisar seus dados históricos de registro. Você deseja ajudá-los a encontrar uma solução que atenda suas necessidades.\nO que você deve fazer?",-->

"options": [

{

"text": "A. Direct them to download and install the Google StackDriver logging agent",   <!--Oriente-os a baixar e instalar o agente de registro do Google StackDriver",-->

"explanation": "This answer might be too presumptive. The team hasn't yet defined their specific requirements for the logging tool, and while Google StackDriver (now part of Google Cloud's Operations suite) is a powerful tool, it may not necessarily meet their unique needs without first understanding those needs.",  <!--"Esta resposta pode ser muito presunçosa. A equipe ainda não definiu seus requisitos específicos para a ferramenta de registro e, embora o Google StackDriver (agora parte do pacote de operações do Google Cloud) seja uma ferramenta poderosa, pode não necessariamente atender às suas necessidades exclusivas sem primeiro entendendo essas necessidades.",-->

"correct": false

},

{

"text": "B. Send them a list of online resources about logging best practices", <!--Envie-lhes uma lista de recursos on-line sobre as melhores práticas de registro",-->

"explanation": "While educating the team on logging best practices is beneficial, it doesn't directly address their immediate need to find a better tool for capturing errors and analyzing log data. This option lacks the hands-on support that the team may require to find a solution.",   <!--Embora educar a equipe sobre as melhores práticas de registro seja benéfico, isso não atende diretamente à necessidade imediata de encontrar uma ferramenta melhor para capturar erros e analisar dados de registro. Essa opção carece do suporte prático que a equipe pode precisar para encontrar um solução.-->

"correct": false

},

{

"text": "C. Help them define their requirements and assess viable logging tools",   <!--Ajude-os a definir seus requisitos e avaliar ferramentas de registro viáveis"-->

"explanation": "This is the most appropriate approach because it ensures that the team first understands their specific needs and requirements. Once these are defined, they can then evaluate different logging tools against these requirements to find the most suitable one. This method is thorough and ensures that the chosen tool will effectively meet their needs.",   <!--Esta é a abordagem mais apropriada porque garante que a equipe primeiro entenda suas necessidades e requisitos específicos. Uma vez definidos, eles podem avaliar diferentes ferramentas de registro em relação a esses requisitos para encontrar a mais adequada. Este método é completo e garante que a ferramenta escolhida atenderá efetivamente às suas necessidades.-->

"correct": true

},

{

"text": "D. Help them upgrade their current tool to take advantage of any new features",  <!--Ajude-os a atualizar sua ferramenta atual para aproveitar todos os novos recursos-->

"explanation": "Upgrading the current tool could be a viable solution, but it assumes that the existing tool, with new features, can meet their needs. Without first understanding their specific requirements, this approach might not solve their problems and could potentially lead to wasted effort if the current tool remains inadequate even after an upgrade.",   <!--Atualizar a ferramenta atual pode ser uma solução viável, mas pressupõe que a ferramenta existente, com novos recursos, possa atender às suas necessidades. Sem primeiro compreender os seus requisitos específicos, esta abordagem pode não resolver os seus problemas e pode potencialmente levar a esforços desperdiçados se a ferramenta atual permanece inadequada mesmo após uma atualização."-->

"correct": false

}

]

}

}

}