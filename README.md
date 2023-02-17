# Projeto Final NLP
Projeto final da disciplina de NLP graduação BIA e mestrado UFG

# Autores:
 * Gabriel Urzeda
 * Gabriel Jhordan Gomes de Oliveira
 * Gustavo Barbosa
 * João Paulo Cavalcante Presa
 
 # Instruções
  * Clone o projeto e execute todos os notebooks da pasta iniciar_projeto_gerar_datasets (seguindo as instruções)
  * ATENÇÃO: Para rodar o projeto inicial é preciso instalar as dependências da bibliotea python pdfplumber (requirements) o ImageMagick e o ghostscript
    * Para instalar o ImageMagick no linux basta executar apt-get install libmagickwand-dev depois editar o arquivo policy.xml em /etc/ImageMagick-6/policy.xml
    * Onde está escrito \<policy domain="coder" rights="none" pattern="PDF" /> substitua por \<policy domain="coder" rights="read | write" pattern="PDF" />
    * Caso não seja feito isso não será possível executar o projeto.
    * Para outros sistemas operacionais consultar https://docs.wand-py.org/en/latest/guide/install.html
    * O ghostscript já vem na maioria das distribuições linux, mas caso precise instalá-lo, consulte:
    * https://ghostscript.readthedocs.io/en/latest/Install.html
    * Não instalar essas dependências vai dar erro na hora de gerar as imagens dos pdfs para os projetos de segmentação semântica e layoutlm, caso esteja dando erro nessa etapa verifique se seguiu as instruções acima, relembrando que é preciso alterar o policy.xml como descrito acima no ImageMagick, uma versão do policy.xml alterado pode ser encontrada nos .devcontainer dos demais projetos, apenas o iniciar_projeto não é executado em um container por isso é preciso instalar o requirements.txt e as dependencias do SO ImageMagick e o ghostscript, e alterar o policy.xml do ImageMagick, para permitir acesso a PDFs
  * As demais pastas são projetos que já possuem um .devcontainer (basta abrir usando o vscode) com todas as dependências ncessárias incluindo drivers de gpu para execução
  * Caso deseje executar em outro ambiente abra o Dockerfile dos projetos e instale as dependências
