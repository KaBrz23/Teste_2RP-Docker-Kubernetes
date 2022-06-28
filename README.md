# Teste de Docker e Kubernetes

## Tarefa

- Clusterizar uma aplicação criada pelo candidato que fique exibindo no log do pod a cada vinte segundos um valor de uma secret de Kubernetes.

## Etapas
- [x]  Criar uma aplicação que fique exibindo o valor de uma variável de ambiente do sistema operacional de 20 em 20 segundos, o nome da variável deve ser "TWORPTEST" e o valor desta variável deve ser "true100%".
- [x]  Criar um container usando docker ou outro orquestrador de containers similar.
- [x]  Opcional: fazer o upload da imagem construída para um container registry de preferência. Observação: o valor da variável deve ser exibido no log do container
- [x]  Opcional: Instanciar um cluster kubernetes local usando Minikube, K3D ou similar para criação e testes dos manifestos.
- [x]  Criar manifestos kubernetes incluindo os tipos deployment, service, secret. O deployment deve rodar a imagem docker construida nas etapas anteriores e na secret deve ser adicionado a variável esperada pela aplicação e passada para o container como variável de ambiente.
- [ ]  Bônus (opcional): Fazer um script bash que percorre os namespaces e coleta a secret de cada deployment para comparar se o valor da secret do deployment está sendo exibida no log do container que está rodando a aplicação. Se o valor da secret estiver sendo exibida retornar uma mensagem informando que o container tem um problema de segurança.
