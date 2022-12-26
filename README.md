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

<b>Página de Cadastro > Efetua o cadastro do usuário<b><br>

Input-e-mail > E-mail <br>
Input-text > Nome/Razão Social <br>
Input-text(number only) > CPF ou CNPJ <br>
Input-text(number only) > Celular <br>
Input-password > Senha <br>

Button > Cadastrar <br>


Dados salvos na Tabela_User, juntamente com Data,Horário e Ano do cadastro. <br><br><br>
  

<b>Página de Login > Efetua o login do usuário na plataforma<b> <br>

Input > E-mail <br>
Input > Senha <br>

Ambas páginas, contém ligação com botão "Criar uma conta" e "Já possui conta? Clique aqui!", caso seja preciso oscilar entre uma página ou outra. <br><br><br>



<b>2 - Perfil<b>

Após efetuar Login no sistema, é possível deslogar do mesmo, pelo botão "Sair"
  
  Button-Log-out-User-sessions > Sair
  
  Em seguida, contém os dados exibidos do cadastro efetuado pelo usuário, sendo: Nome/Razão social, CPF/CNPJ, E-mail e Celular.
  
  Os dados são exibidos em inputs-disable para que o usuário possa apenas visualizar e não editar de imediato. Os dois primeiros campos, 








