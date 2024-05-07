# Sistema Avaliação de Artigos

Sistema Web, hospedado na UFN, desenvolvido por alunos do curso de Ciência da Computação, para submissão e avaliação de artigos científicos.

- apps
    - usuario
        tipos: administrador, coordenador de evento, ordinario (submete ou avalia)
        nome
        email (chave primária)
        celular
        cpf
        área (Ciências Humana, Ciências da Saúde, Ciências Sociais, Ciências Tecnológicas)
        instituição
        is_active

        Obs.:
            - usuário faz autocadastro (exceto administrador)

    
    - instituição
        nome
        sigla (opcional)
        cidade
        estado
        país
        is_active


    - evento 
        nome
        tipo (congresso, simpósio, revista, capítulo de livro, ....)
        instituição
        data do evento
        local do evento
        coordenador do evento (usuario)
        data limite de envio de trabalhos
        regras de publicação
            - modelo do documento (arquivo template)
            - quantidade de páginas miníma e máxima
            - conteúdo do texto esperado (introdução, revisão bibliográfica, metodologia, resultados, conclusões)
        is_active
    

    - submissão
        responsável (usuário ordinário)
        coautores (usuários ordinários)
        evento (com data limite de envio de trabalhos aberta)
        data e hora da submissão (capturado automático)
        titulo (pensar no limite de palavras)
        resumo (pensar no limite de caracteres, linhas ou palavras)
        abstract (pensar no limite de caracteres, linhas ou palavras)
        palavras-chave (pensar no limite de palavras)
        categoria ou subárea do trabalho (???)
        arquivo da versão de avaliação (sem autores ou identificação)
        arquivo da versão corrigida e aprovada (com autores ou identificação)
        arquivo do comitê de ética zipado (quando artigo trabalhar com seres humanos)

