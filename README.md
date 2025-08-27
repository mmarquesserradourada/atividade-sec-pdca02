# atividade-sec-pdca02
Atividade Aula Segurança 02 - Faculdade Serra Dourada Lorena

Código a ser analisado em PHP.



if ($_SERVER['REQUEST_METHOD'] == 'POST') {
    $upload_dir = "uploads/";
    $file = $upload_dir . basename($_FILES["file"]["name"]);

    if (move_uploaded_file($_FILES["file"]["tmp_name"], $file)) {
        echo "Arquivo enviado com sucesso!";
    } else {
        echo "Erro ao enviar arquivo.";
    }
}



# O que tem que ser feito
Aplicação do PDCA

🔹 Plan (Planejar)
Identificar vulnerabilidades no código acima.
Analisar riscos (Probabilidade x Impacto) de exploração.

Criar tabela de riscos.

🔹 Do (Executar)
Corrigir código (citar quais são as correções feitas)

🔹 Check (Verificar)
Testar novamente o sistema.
Verificar se as vulnerabilidades foram mitigadas.

🔹 Act (Agir)
Atualizar documentação no repositório GIT, criar um arquivo VALIDAÇÃO-NOME.log
Criar boas práticas de segurança (citar detalhadamente quais são).


## Subir versão corrigida para o GitHub respondendo abaixo os itens:

Questionário para os alunos

Quais vulnerabilidades você encontrou no código original?

Qual vulnerabilidade apresentou maior risco (P x I)?

Qual seria o impacto real se essa falha fosse explorada em uma empresa?

Como você corrige as falhas encontradas?

Após aplicar o PDCA, quais melhorias foram efetivas?

## Vocês Alunos deverão fazer:
Fork: O aluno faz um "fork" do seu repositório. Isso cria uma cópia completa do seu projeto na conta dele. O repositório original é chamado de "upstream" e a cópia do aluno é o "origin".

Clone e Trabalho: O aluno clona a cópia dele (o "origin") para a máquina local e faz as alterações no código.

Commit e Push: Após as alterações, o aluno faz um "commit" e envia (push) as mudanças para o repositório dele no GitHub.

Pull Request: O aluno abre um Pull Request do repositório dele (o "origin") para o seu repositório original (o "upstream").
