Eu me esforcei muito e dei o meu melhor para fazer este projeto! Espero que atenda minimamente as expectativas por alguma coisa (OBS: Infelizmente o DELETE não está funcionando :-(  )

-
-
-
-
-
-

Em primeiro lugar, ao baixar o arquivo aqui pelo GitHub acredito que o arquivo deve estar compactado. Então clique com o botão direito do mouse, e descompacte o mesmo. 
Entre no VSCODE (se não tiver, faça o download do programa: https://code.visualstudio.com/Download), e no VSCODE abra a pasta do arquivo descompactado. 
E então abra o campo de terminal do VSCODE, no terminal ative a venv do programa com o comando "  ./venv/Scripts/activate" (recomendo copiar e colar esse comando que botei aí), e então ative o servidor DJANGO com o comando "py manage.py runserver".
Espere, e após ativado o servidor digite esta URL no seu navegador:

http://127.0.0.1:8000/api/pessoas/CRUD/

Nesta URL podem ser feito os métodos CRUD (Create, Read, Update e Delete), em que no 1° campo você pode pôr estes 2 testes abaixo para adicionar os profissionais clicando no botão "POST":

{
        "person_id": "1",
        "person_name": "joao",
        "person_profession": "enfermeiro",
        "person_address": "Campo Grande",
        "person_contact": "21992020071"
    }

    {
        "person_id": "2",
        "person_name": "luan",
        "person_profession": "medico",
        "person_address": "Santa Cruz",
        "person_contact": "2198711243"
    }

E no 2° campo você pode editar algum destes 2 testes acima, repetindo o "person_id" que você quer mudar. 
Por exemplo, se você quiser modificar a base de dados person_id 1 que tem nome de joão, profissão de endereço e etc, mantenha o "person_id": "1" como tá abaixo:
    {
        "person_id": "1",
        "person_name": "roberto",
        "person_profession": "cirurgiao",
        "person_address": "Olinda",
        "person_contact": "2199308723"
    }

MAS se você quiser mudar a base de dados person_id 2 que tem aquele nome de luan, profissão médico e etc, digite "2" no campo de "person_id" como tá abaixo:

{
        "person_id": "2",
        "person_name": "antonio",
        "person_profession": "pediatra",
        "person_address": "caxias",
        "person_contact": "2198556024"
    }

Para ter acesso e vizualizar todos os profissionais por meio do método GET, vá para esta URL:
http://127.0.0.1:8000/api/pessoas

-
-
-
-
-
-

Digite agora esta URL no navegador:

http://127.0.0.1:8000/api/consultar/CRUD/

Nesta URL podem ser feito os métodos CRUD (Create, Read, Update e Delete), em que no 1° campo você pode pôr estes 2 testes abaixo para adicionar as consultas clicando no botão "POST":

Testes para adicionar consultas: "Método POST":
    {
        "consultation_id": "1",
        "consultation_data": "2024-04-12",
        "consultation_person": "joao"
    }

     {
        "consultation_id": "2",
        "consultation_data": "2024-04-13",
        "consultation_person": "luan"
    }
    
E no 2° campo você pode editar algum destes 2 testes acima, repetindo o "consultation_id" que você quer mudar. 
Por exemplo, se você quiser modificar a base de dados consultation_id 1 que tem nome do profissional vinculado a consulta como "joao", mantenha o "consultation_id": "1" como tá abaixo:

{
        "consultation_id": "1",
        "consultation_data": "2024-07-12",
        "consultation_person": "alexandre"
    }

MAS se você quiser mudar a base de dados person_id 2 que tem aquele nome do profissional vinculado a consulta como "luan", digite "2" no campo de "consultation_id" como tá abaixo:

{
        "consultation_id": "2",
        "consultation_data": "2024-04-15",
        "consultation_person": "roberto"
    }

Para ter acesso e vizualizar todos as consultas por meio do método GET, vá para esta URL:
http://127.0.0.1:8000/api/consultas

-
-
-
-
-
-

Qualquer dúvida, feedback, pergunta, ou qualquer outra coisa estou a disposição! Espero ter agradado em pelo menos alguma coisa.
