## Conhecendo o AWS IAM

 - O AWS Identity and Access Management permite o gerenciamento seguro do acesso aos serviços e recursos da AWS por criação de usuários, grupos e permissões.


## Recursos do IAM

 - Acesso compartilhado a contas da AWS: permissão de acesso a outros usuários.

 - Permissões granulares: diferentes níveis de acesso de acordo com as funções dos usuários em uma conta AWS.

 - MFA: Autenticação de múltiplos fatores.

 - Identidades federadas: credenciais podem ser importadas de outros provedores de identidade. Como por exemplo a conta do google pode ser usada para identificação.

 - Integração com serviços AWS: estabelece níveis de permissões de acesso aos serviços AWS.

 - Gratuito: o IAM não possui custos ou limites de uso.


## Termos e conceitos do IAM

 - Identity: fornece acesso a uma conta na AWS. Tudo que determina acesso a conta AWS. Exemplo: usuário, políticas de acesso, role(função de usuário).

 - IAM Users: representa uma pessoa ou serviço o que utiliza serviços AWS.

 - User Groups: coleção de usuários IAM. Usado para separar grupos de usuários dentro de uma empresa, cada grupo pode ter suas permissões de acesso.

 - IAM Roles: conjunto de permissões que determinam o nível de acesso de uma identidade aos serviços AWS. O que uma identidade pode fazer dentro da AWS. Pode ser Inline policy que permite atrelar roles diretamente a uma identidade (não são reaproveitáveis) ou Managed policy que é um conjnto de permissões disponíveis para várias identidades. A Inline policy é específica enquanto a managed pode ser replicada e estendida a várias identidades. 


## IAM Policies

 - Descrita no formato JSON, define permissões de acesso a serviços AWS.

 - IAM Permissions: nível mais baixo da hierarquia, determina se uma identidade pode ou não toamr uma ação sobre um recurso na AWS (Allow/Deny).

 - Exemplo de policy: ```{
    "Version": "2012-10-17",
    "Statement":{
        "Effect": "Allow",
        "Action": "s3:ListBucket",
        "Resource": "arn:aws:s3:::example_bucket"
     }
    }```


## Boas práticas

 - A AWS tem uma lista de melhores práticas para ajudar desenvolvedores e profissionais de TI a gerenciar o acesso aos recursos da AWS.

 - Conta root: não utilizar em tarefas diárias de desenvolvimento, para evitar problemas como faturas muito caras ou quebrar todo o sistema.

 - Usuários: crie usuários individuais.

 - Privilégios mínimos: prover somente o nível de acesso necessário para os usuários.

 - Permissões: utilizar grupos de usuários com permissões para tal grupo.

 - Auditoria: ativar o AWS CloudTrail. Captura todos os logs, qualquer tipo de acesso dentro da AWS.

 - Senhas: utilizar senhas fortes.

 - MFA: ativar para usuários privilegiados.