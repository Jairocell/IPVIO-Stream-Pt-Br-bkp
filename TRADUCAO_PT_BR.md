# Português do Brasil (pt-BR) — IPVIO Stream

Esta alteração adiciona `pt` à lista de idiomas do aplicativo, apresenta o nome `Português (Brasil)`, reconhece automaticamente o idioma do Android quando configurado como `pt`/`pt-BR`, seleciona `pt-BR` nas consultas ao TMDB e disponibiliza traduções brasileiras para os textos incluídos em `DictPt.kt` e `DictPtW`.

## Importante sobre a cobertura

O projeto possui um catálogo extenso de textos de interface. Nesta primeira implementação foram traduzidas as entradas de interface prioritárias e as novas entradas do bloco Wishbox. Textos ainda não contemplados pelo dicionário português continuam usando o fallback em inglês definido pelo mecanismo original, em vez de exibir uma tradução inventada ou quebrar a interface. Portanto, a tradução está integrada funcionalmente, mas ainda não representa cobertura integral de todos os textos do aplicativo.

## Validação

Foi incluído teste unitário para reconhecimento de `pt-BR`, nome nativo, traduções essenciais e preservação de placeholder. A execução dos testes não pôde ser concluída neste ambiente porque o Gradle Wrapper precisa baixar o Gradle 9.6.0 e o ambiente está sem acesso à internet (`UnknownHostException: services.gradle.org`).
