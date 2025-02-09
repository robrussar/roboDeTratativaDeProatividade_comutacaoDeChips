# roboDeTratativaDeProatividade_comutacaoDeChips

Robô de Tratativa de Proatividade

Ao detectarmos nas ferramentas existentes que a comunicação de um link estava com instabilidade e/ou indisponibilidade insatisfatória, o sistema abria um chamado de proatividade.
A tratativa de proatividade era para todos os links, tanto para links moveis (modens 3G e 4G), quanto para links fixos (metálico, fibra óptica e satélites)

Então fazíamos manualmente durante o dia, entre nossas atividades um troubleshooting completo nos links.
Surge então a possibilidade de fazer um robô para realizar a tratativa com um tempo otimizado.  Essa tratativa durante o dia, demandava entre 10 a 20 minutos, pois nos modems móveis precisávamos comutar os chips, os roteadores de comunicação móvel funcionavam com dois chips de operadores diferentes, um chip Vivo, Claro ou Tim, ou seja, se modem estava funcionando no chip 1 tínhamos que verificar se o chip 2 estava funcionando, então fazíamos a comutação. Essa comutação demorava alguns minutos para assumir a comunicação no outro chip, isso que era demorado. Caso não funcionasse abríamos chamado para resetar o chip ou trocar o modem. 

Fiz 3 robos, um para routers da Tbnet-Fortnet, outro para routers da Cisco 4G e outro para routers Cisco 3G.

Visando a otimização da mão de obra, o robô rodava durante toda a noite, captando todos os testes e salvando em um bloco de notas os resultados, como:  temperatura, sinal dos chips, se ambos os chips estavam operantes, tabela arp, tempo logado (uptime) e ping (latência e perda de pacotes). Consequentemente, já tínhamos o troubleshooting pronto, então pegamos os resultados e dávamos as tratativas necessárias durante o dia como teste ok, modem inoperante, algum chip inoperante, quedas por energia elétrica, quedas por desligamento do estabelecimento, dentre outras. Isso otimiza muito o tempo de tratativa da atividade, pois como tínhamos muitas outras tarefas a fazer ao mesmo tempo, fazer essa tratativa era muito custosa pois tinham outras atividades mais urgentes para tratar e sempre éramos interrompidos no meio da tratativa de proatividade. 

No vídeo temos o código do modem da Tbnet-Fortnet. Não tenho os outros códigos pois não postei enquanto trabalhava na empresa, mas esse serve de base pois é o mesmo funcionamento. 

Usamos Pyperclip, Regex e PyAutoGui. 
