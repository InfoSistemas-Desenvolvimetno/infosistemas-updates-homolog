# InfoSistemas - canal de atualizacoes (HOMOLOGACAO)

Este repositorio e o canal de **HOMOLOGACAO**. **Nenhuma instalacao de loja deve apontar para ele.** As versoes aqui ainda estao em teste. O canal oficial de atualizacoes do sistema InfoSistemas (PDV e
Retaguarda). O Atualizador instalado em cada loja consulta este repositorio para saber se ha
versao nova e de onde baixa-la.

> **Repositorio publico por necessidade tecnica.** O Atualizador le o `version.json` sem
> autenticacao. Aqui ficam apenas o arquivo de versao e os pacotes de instalacao - **nao ha
> codigo-fonte, dado de cliente nem informacao de operacao neste repositorio.**

---

## Como funciona

| | |
|---|---|
| **`version.json`** | diz qual e a versao vigente, onde esta o pacote e o que mudou. **E o gatilho**: o Atualizador compara com a versao instalada e so oferece atualizacao se a daqui for maior |
| **Releases** | cada versao publicada tem uma release com o pacote `InfoSistemas-Update-<versao>.zip` anexado. Quando ha aplicativo Android novo, o `.apk` assinado acompanha a mesma release |

### O campo `mandatory`

Quando `false`, a atualizacao e oferecida e **quem decide o momento e a loja**. O Atualizador
nao interrompe operacao nem atualiza sozinho: alguem precisa abri-lo e mandar atualizar.

---

## Para quem opera uma loja

1. **Feche o sistema** (Frente de Caixa, Mapa de Mesas, Retaguarda).
2. Abra o **Atualizador** e clique em atualizar.
3. **Prefira fazer isso fora do horario de movimento.** Os pacotes tem centenas de megabytes.

Se a atualizacao falhar, o Atualizador informa a causa - rede, servidor, espaco em disco ou
cancelamento. **Clicar de novo e sempre seguro.**

---

## Para quem da suporte

- **Baixar o pacote manualmente:** use o `.zip` anexado a release da versao desejada.
- **Aplicativo Android:** quando ha versao nova, o `.apk` assinado esta na mesma release.
- **Saber o que mudou:** o texto de cada release descreve as mudancas em linguagem de operacao.

---

## O que este repositorio NAO e

| | |
|---|---|
| **nao e o codigo-fonte** | o fonte do sistema e privado |
| **nao e canal de suporte** | duvidas e chamados nao sao tratados aqui |
| **nao aceita contribuicao externa** | o conteudo e gerado pelo processo de release da InfoSistemas |

---

## Canal de homologacao

Existe um canal separado, usado para testar cada versao antes de as lojas a receberem. **Uma
instalacao de loja nunca deve apontar para ele.**
