# DesafioBubbleEduzz


  O produto foi desenvolvido para resolver um problema real da sua própria área, que contenha
Criação/Atualização de registros (salvando dados no banco de dados do Bubble), Leitura de dados e
exibição em formato tabela/grid e exclusão de dado.

Na página inicial da sua aplicação, exibe a temperatura da cidade de Sorocaba (faça uma integração
com uma das APIs de meteorologia disponíveis na plataforma para que o valor esteja sempre
atualizado.


Logo, o problema foi identificado, "falta autonomia de alteração de e-mail pelo prórpio cliente da Eduzz", embora a alteração de e-mail em nossa plataforma seja efetuada internamento pelos atendentes, a mesma não trás produtividade e gera altas demantas, atingindo todos núcleos dentro da área. Atualmente a atualização de dados cadastrais em nossa plataforma é efetuada via ticket/chat, onde ocorre um fluxo de atendimento para que seja concretizada a modificação. Esse fluxo, persiste em diversas etapas, solicitando documentos e fotos para que seja realizada com sucesso. Entretando, ocasiona em diversos fatores, principalemnte no quesito produtividade/qualidade.

O proejto trás uma automação para alteração de dados sensíveis, uma página onde ocorre a moderação das solicitações dos dados. 

O usuário, seja ele qual for (Cliente Final, Afiliado ou Produtor), efetua o processo de solicitação, enviando os documentos, fotos e e-mail que deseja inserir na plataforma.

Fluxos efetuados:<br><br><br> 

<b>1 - Cadastro / Login<b>


Em primeiro lugar, para efetuar a solicitação de alteração é preciso estar logado no sistema, para isso, possuí á página de Cadastro e Login.<br>

      1.1 Página de Cadastro > Efetua o cadastro do usuário

      Input-e-mail > E-mail
      Input-text > Nome/Razão Social 
      Input-text(number only) > CPF ou CNPJ 
      Input-text(number only) > Celular
      Input-password > Senha

      Button > Cadastrar  -- Redirecionando para á página Perfil


      Dados salvos na Tabela_User, juntamente com Data,Horário e Ano do cadastro.
  

      1.2 Página de Login > Efetua o login do usuário na plataforma

      Input > E-mail 
      Input > Senha 
  
      Botão > Login -- Redirecionando para á página Perfil

      Ambas páginas, contém ligação com botão "Criar uma conta" e "Já possui conta? Clique aqui!",
      caso seja preciso oscilar entre as páginas.



<b>2 - Perfil<b>

  Após efetuar Login no sistema, é possível deslogar do mesmo, pelo botão "Sair"
  
  Button-Log-out-User-sessions > Sair
  Cliente no mesmo, é encaminhado para a página principal onde contém informações sobre "Temperatura da Cidade de Sorocaba", consumida pela API:         (https://api.hgbrasil.com/weather?woeid=455913), disponibilizada pelo próprio Bubble.io
  
  Efetuando Login novamente, contém os dados exibidos do cadastro efetuado pelo usuário, sendo: Nome/Razão social, CPF/CNPJ, E-mail e Celular.
  
  Os dados são exibidos em inputs-disable para que o usuário possa apenas visualizar e não editar de imediato. 
  
  ![image](https://user-images.githubusercontent.com/85848930/209582923-8a8fa242-baa4-43f2-b601-90415224fc36.png)

  
  O "input-text(number only)> Celular", é possível efetuar alteração sem precisar validar documentos/fotos dos clientes. Basta clicar no ícone de edição e inserir o celular que desejar.
  
  Já o campo, E-mail, é necessário efetruar diversos procedimentos por se tratar de um dado sensível. <br><br><br>



  3 - Solicitação de alteração de e-mail
  
  Essa página contém solicitações de documentos/informações dos clientes. 
  
    3.1 Solicitar que o mesmo autorize ou rejeite o tratamento dos dados na plataforma, se atentando as leis LGDP
        (Lei Geral de Proteção de Dados)
  
        É fundamental que o mesmo escreva se autoriza ou não e o motivo pelo qual está solicitando a edição do e-mail.


    3.2 Logo em seguida, é solicitado 4 fotos para a aprovação da edição.
    
    3.3 Informar o e-mail que deseja inserir na plataforma.
  
![image](https://user-images.githubusercontent.com/85848930/209583594-e0156287-480c-428e-843f-b5784bb74d35.png)


    Finalizando com um Botão para salvar e armazenar todos as informações/documentos na Tabela_Dados.
    Sendo eles: Arquivo1, Arquivo2, Arquivo3, Arquivo4, Descrição, E-mail_Novo e Data de solicitação.
  
    Clicando no Botão "Enviar solicitação" o usuário é redirecionado para a página Perfil, onde é notificado e informado 
    que efetuou a solicitação de alteração.
  
  
 4 - Validação de alteração
  
  Essa página, fica disponibilizada para os atendentes (admin), onde o usuário não possuirá acesso.  
  
  
  Puxando informações da Tabela_Dados, que o usuário cadastrou sua solicitação:
  
  ![image](https://user-images.githubusercontent.com/85848930/209583843-1236325f-831e-4f62-93fb-4e5f4559ed63.png)

  Descrição, E-mail deseja, CPF do cadastro, e documentos solicitados. 
  
  Os atendentes, irão visualizar a solicitação e vericar diante aos documentos/descrição podendo APROVAR ou REPROVAR a solicitação. 
  
    4.1 Após clicar no Botão APROVAR, o e-mail do cadastro do usuário é alterado com sucesso e os dados armazenados na
        Tabela_Dados é excluído, referente a essa solicitação.
  
        Caso clique em REPROVAR, o e-mail não é alterado e os dados armazenados na Tabela_Dados é excluído, referente a essa solicitação.
  
        Logo em seguida, contém um Botão para retornar a página de Perfil do Usuário, onde é possível visualizar o e-mail alterado ou reprovado.
  
 5 - Justificativa 

    Dentro da área do atendimento, possuímos diversos Núcleos, sendo eles: Nutror Plus ++, Órbita e Check-out, esse automatização iria impactar todos núcleos, possuindo benefícios para todos.
  
  
  Att, José Henrique Freitas (Zé) ;) 
