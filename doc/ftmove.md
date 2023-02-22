## ftmove(filetomove)

# features
 ftmove-(
    funcionalidades do momento:{
        *mover e copiar arquivos, comando deve ser executado na pasta pois o script ele pega a pasta atual onde o usuário está dentro do terminal.

        *mover e copiar multiplos arquivos através de uma única palavra chave

        *deletar multiplos arquivos através de uma palavra chave
    },

    Funcionalidades futuras{
        adicionar metodos onde o usuário poderá salvar caminhos que ele usa com frequência dentro do script, o script irá pegar um arquivo onde estará armazenado isso, pensei em colocar em json para ter chave e o objeto, ai o usuário poderá colocar o nome da chave assim sendo melhor para lembrar o nome que deu ao diretório. Essa funcionalidade vai ser útil para que o usuário não precise sempre estar na pasta do arquivo para move-lo, ou sempre ter que ficar digitando o diretório completo
    }
);

# Para saber como usar o programa no seu terminal basta só digitar "ftmove" e dar um enter para ler a ajuda, por enquanto a ajuda está apenas em Inglês por lá mas vou disponibilizar como usar por aqui também em português

## como usar
    ftmove -transfer{
    TRANSFERE ARQUIVOS DE UMA PASTA PARA OUTRA PEGANDO O SEU DIRETÓRIO ATUAL E ENVIANDO PARA OUTRO DIRETÓRIO QUE ESPECÍFICOU COMO POR EX: ftmove -transfer <nomearquivo.extensão> <caminho\de\destino> 

    O ARQUIVO QUE DIGITOU IRÁ PARA O DIRETÓRIO PASSADO DE DESTINO. NÃO PRECISA NEM COLOCAR A "\" NO FINAL POIS NO SCRIPT ADICIONA UMA AUTOMATICAMENTE.

    LEMBRANDO QUE VOCÊ DEVE ESTAR NA PASTA DO ARQUIVO EXISTENTE PARA FAZER ISSO, NÃO IRÁ ADIANTAR PASSAR O DIRETÓRIO ATUAL POIS O SCRIPT JÁ ADICIONA AUTOMÁTICAMENTE O DIRETORIO QUE ESTÁ NO MOMENTO, E NÃO É POSSÍVEL PASSAR O DIRETÓRIO QUE O ARQUIVO ESTÁ POIS NÃO ESTÁ PROGRAMADO PRA PASSAR O DIRETÓRIO DE ORIGEM EM ARGUMENTO
}

ftmove -copy{
    COPIA ARQUIVOS DE UMA PASTA PARA OUTRA PEGANDO O SEU DIRETORIO ATUAL E COLANDO PARA O OUTRO DIRETÓRIO QUE ESPECIFICOU COMO POR EX: ftmove -copy <nomearquivo.extensão> <caminho\de\destino>

    O ARQUIVO QUE DIGITOU IRÁ PARA O DIRETÓRIO PASSADO DE DESTINO. NÃO PRECISA NEM COLOCAR A "\" NO FINAL POIS NO SCRIPT ADICIONA UMA AUTOMATICAMENTE.

    LEMBRANDO QUE VOCÊ DEVE ESTAR NA PASTA DO ARQUIVO EXISTENTE PARA FAZER ISSO, NÃO IRÁ ADIANTAR PASSAR O DIRETÓRIO ATUAL POIS O SCRIPT JÁ ADICIONA AUTOMÁTICAMENTE O DIRETORIO QUE ESTÁ NO MOMENTO, E NÃO É POSSÍVEL PASSAR O DIRETÓRIO QUE O ARQUIVO ESTÁ POIS NÃO ESTÁ PROGRAMADO PRA PASSAR O DIRETÓRIO DE ORIGEM EM ARGUMENTO
}

ftmove -fstmove -transfer{
    ESSA FUNÇÃO SERVE PARA VOCÊ MOVER ARQUIVOS EM CADEIA COM UMA PALAVRA CHAVE QUE VOCÊ ESCOLHER, COMO POR EX: ftmove -fstmove -transfer <palavra_chave> <caminho\de\origem> <caminho\de\destino>

    TODOS OS ARQUIVOS QUE CONTIVER "palavra_chave" IRÃO SER TRANSFERIDOS PARA A PASTA DE DESTINO QUE DESEJOU
}

ftmove -fstmove -copy{
    ESSA FUNÇÃO SERVE PARA VOCÊ COPIAR ARQUIVOS EM CADEIA COM UMA PALAVRA CHAVE QUE ESCOLHER, COMO POR EX: ftmove -fstmove -copy <palavra_chave> <caminho\de\origem> <caminho\de\destino> 

    TODOS OS ARQUIVOS QUE CONTIVER "palavra_chave" IRÃO SER TRANSFERIDOS PARA A PASTA DE DESTINO QUE VOCÊ DESEJOU
}

ftmove -fstmove -delete{
    ESSA FUNÇÃO SERVE PARA DELETAR ARQUIVOS EM CADEIA COM UMA PALAVRA CHAVE QUE ESCOLHER, COMO POR EX: ftmove -fstmove -delete <palavra_chave> <caminho\arquivos\que\serão\deletados>

    TODOS OS ARQUIVOS DESSA PASTA QUE INDICOU QUE CONTÉM "palavra_chave" SERÃO DELETADOS PERMANENTEMENTE!
}