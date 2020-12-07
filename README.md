# Trabalho de graduação

## 1 Introdução;

A maioria das pessoas, não calculam a quantidade de combustível para o trajeto desejado e como resultado acabam ficando sem combustível no meio do caminho, chamado popularmente de pane seca (Brasil Postos, 2017). Durante a pane seca há diversos problemas envolvidos, um dos mais críticos é a segurança que pode variar de acordo com o horário da pane e a movimentação da via. Devido a esta situação muitas pessoas utilizam reservatórios PEAD (Polietileno de alta densidade) para transportar combustível, o que não é aconselhado por não estar nos padrões exigidos pelo Inmetro (Brasil Postos, 2014).

O utilização da embalagem incorreta pode elevar o problema da pane seca devido aos perigos no transporte do combustível. O risco de uma carga estática gerar combustão no combustível contido no recipiente, ou o mesmo ser degradado devido a radiação ultravioleta danificando o veículo abastecido (Ferreira, 2017).


## 1.1 Objetivos

O projeto tem como objetivo o desenvolvimento de um sistema de delivery de combustível. Este tipo de transporte muitas vezes é feito pelo próprio consumidor que majoritariamente não tem conhecimento das regulamentações exigidas na norma ABNT NBR 15.594-1: 2008 para o transporte de combustível (Brasil Postos, 2014).

O sistema terá três tipos de usuários: colaboradores, fornecedores e cliente. O colaborador seram os usuários responsávei pela entrega do combustível aos clientes, o fornecedor será o usuário responsável pelo fornecimento do combustível e o cliente será o usuário responsável por fazer o pedido e receber o combustível.

O colaborador só poderá atuar após completar uma série de cursos de como transportar o combustível da maneira correta (método exigido pela norma ABNT NBR 15.594-1: 2008). Estes cursos serão aplicados pelo software através do acesso de colaborador.

## 2. Fundamentação Técnica

Para o desenvolvimento técnico deste projeto, será utilizado API's para localização (geolocalização) e plataforma de pagamento online do cliente, fornecedor e colaborador.
Para o desenvolvimento do sistema será utilizado REST API e para desenvolvimento da aplicação utilizarei Dart com o framework Flutter.

### 2.1 Localização

Através de um satélite é obtido a localização geográfica de um dispositivo que precisa ter conexão com a internet para se tornar visível.
Neste projeto a geolocalização será usada nos três tipos de usuários (colaborador, fornecedor e cliente).
No colaborador, a geolocalização terá como principal função mostrar onde o fornecedor e o cliente estão para que possa ser feito o transporte do combustível para o destino final.
No fornecedor, a geolocalização atuará mostrando a distância entre o própio fornecedor e colaborador, mostrará também a distância até o cliente.
No cliente, a geolocalização terá o papel de mostrar a distância entre o própio cliente e colaborador.
