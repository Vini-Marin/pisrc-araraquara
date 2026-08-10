## Escreva uma benchmark para uma supermercado online o Quitandinha online 10/08 com dois casos ao menos.
Benchmark de Segurança e Confiabilidade em um Supermercado Online
Caso de Negócio
A empresa Quitandinha Online é um supermercado virtual que atende aproximadamente 8.000 clientes por dia. Durante promoções e datas comemorativas o número de acessos cresce significativamente, causando lentidão, indisponibilidade do sistema e tentativas de ataques ao sistema e sua base de dados.
Com o aumento das reclamações e da perda de vendas, a empresa decidiu realizar um benchmark para avaliar a infraestrutura atual e identificar melhorias relacionadas à Segurança e à Confiabilidade do ambiente.
O objetivo é reduzir falhas, aumentar a disponibilidade do sistema e garantir a proteção de dados e informações dos clientes.
________________________________________
Workload
O workload representa o comportamento típico dos usuários durante um momento de pico de uso do sistema.
Características
•	8.000 usuários ativos por dia; 
•	Até 2.000 usuários simultâneos em horários de pico; 
•	Aproximadamente 200 requisições por segundo. 
Operações simuladas
•	Login de clientes; 
•	Pesquisa de produtos; 
•	Consulta de ofertas; 
•	Inclusão de produtos no carrinho; 
•	Atualização do carrinho; 
•	Finalização da compra; 
•	Pagamento online; 
•	Consulta do histórico de pedidos. 
________________________________________

Benchmark 1 – Segurança
Objetivo
Avaliar a capacidade da infraestrutura em proteger os dados dos clientes e manter o funcionamento da aplicação diante de acessos maliciosos.
Ambiente
•	Servidor Linux Ubuntu; 
•	Servidor Web Nginx; 
•	Banco de Dados MySQL; 
•	Firewall; 
•	Certificado HTTPS (TLS 1.3); 
•	Autenticação JWT; 
•	Web Application Firewall (WAF). 
Métricas
Métrica	Objetivo
Tempo médio de autenticação	Menor que 300ms
Tentativas de acesso bloqueadas	Maior que 99%
Incidentes de segurança	Zero

Disponibilidade do login	99,9%

Resultado esperado
A aplicação deve manter o tempo de resposta abaixo de 300ms e impedir acessos não autorizados sem comprometer o desempenho. Além de ter a capacidade de atender a todos os clientes tentando acessar, deixando o site sempre disponível e seguro.
________________________________________

Benchmark 2 – Confiabilidade
Objetivo
Verificar a estabilidade da aplicação durante períodos de alta demanda, garantindo que os clientes consigam finalizar suas compras sem interrupções.
Ambiente
•	Dois servidores de aplicação; 
•	Balanceador de carga; 
•	Banco de Dados replicado; 
•	Backup automático; 
•	Monitoramento contínuo. 
Métricas
Métrica	Objetivo
Disponibilidade	99,95%
Tempo médio de resposta	Menor que 200ms
Perda de transações	Zero
Tempo de recuperação após falha	Menor que 5 minutos
Resultado esperado
Mesmo durante promoções com milhares de acessos simultâneos, o sistema deve permanecer disponível, sem perda de pedidos e com tempo de resposta menor que 200ms.
________________________________________
Ferramentas Utilizadas
•	Apache JMeter (simulação de carga); 
•	Grafana (monitoramento); 
•	Prometheus (coleta de métricas); 
•	Docker (virtualização dos serviços); 
•	MySQL (banco de dados); 
•	Nginx (servidor web e proxy reverso). 
________________________________________
Conclusão
O benchmark demonstrou que investir em Segurança e Confiabilidade é fundamental para um supermercado online. A adoção de mecanismos como HTTPS, autenticação segura e firewall protege as informações dos clientes, enquanto a utilização de balanceamento de carga e monitoramento garante alta disponibilidade do serviço.
Com essas melhorias, é esperado diminuir as interrupções, evitar perdas financeiras em momentos de grande demanda e proporcionar uma experiência de compra mais segura e confiável para os clientes.
