Site do trabalho acadêmico "Inteligência Artificial e Machine Learning: conceitos, aplicações e desafios", feito para o 1º semestre de 2026 do curso de Tecnologia em Análise e Desenvolvimento de Sistemas da UCDB (turma 262, noturno).

O site é uma página única com tema escuro. Ele reúne o trabalho escrito (introdução, objetivos, metodologia, fundamentação teórica, resultados, relação com as disciplinas, considerações finais, referências) e a entrevista feita com um especialista da área.

## Como abrir

Não precisa instalar nada. Salve o arquivo HTML como `index.html` e abra no navegador.

O site carrega Bootstrap, Font Awesome, Google Fonts e AOS por links externos (CDN). Sem conexão com a internet, a página abre sem estilo, sem ícones e sem animações.

## O que tem no projeto

Um único arquivo HTML, com o CSS e o JavaScript dentro dele.

As seções ficam em ordem na página e cada uma tem um `id` usado como âncora: `capa`, `sumario`, `introducao`, `objetivos`, `metodologia`, `fundamentacao`, `resultados`, `disciplinas`, `produto`, `consideracoes`, `referencias` e `apendice`. A barra fixa do topo e o sumário apontam para esses ids.

O JavaScript faz quatro coisas:

- liga a biblioteca AOS, que anima os blocos conforme a rolagem;
- deixa a barra de navegação mais compacta depois de 80 px de rolagem e mostra o botão de voltar ao topo depois de 600 px;
- marca no menu a seção em que o leitor está;
- faz a rolagem suave até a âncora clicada, descontando a altura da barra fixa, e fecha o menu no celular.

## Tecnologias

HTML5, CSS3, JavaScript, Bootstrap 5.3.2, Font Awesome 6.4.2, Google Fonts (Inter, Space Grotesk e Merriweather) e AOS 2.3.4.

## Como mudar o visual

As cores, os raios de borda, as sombras e as transições estão como variáveis CSS no bloco `:root`, no começo do `<style>`. Para trocar a cor de destaque, por exemplo, altere `--accent` (e `--accent-glow`, que é a mesma cor com transparência). O resto do site usa essas variáveis.

Para incluir uma seção nova, copie uma das existentes, troque o `id` e adicione um link para ela no menu e no sumário.

## Pontos para revisar

Esses detalhes não impedem o site de funcionar, mas vale corrigir:

- Na seção 4.6 estão escritos "propunção" e "Conexista". Os termos corretos devem ser "proposição" e "Conexionista".
- O ícone do Font Awesome na lista de tecnologias usa `fas fa-font-awesome`. Como é um ícone de marca, o certo é `fab`.
- O ponto verde do link ativo no menu usa posicionamento absoluto, mas `.nav-link` não tem `position: relative`. O ponto pode aparecer fora do lugar.
- O menu do celular é fechado removendo a classe `show` na mão. O mais seguro é usar o `collapse` do próprio Bootstrap.
- A rolagem suave está declarada no CSS (`scroll-behavior`) e também no JavaScript. Um dos dois basta.

## Como o código foi feito

O código-fonte foi gerado com a ferramenta de IA Deepseek V4 e depois revisado e adaptado pela equipe. O prompt usado está registrado na seção "Produto desenvolvido" do próprio site.

## Autoria

Trabalho de grupo da UCDB, Campo Grande (MS), 2026.

- Eduardo Henrique Lubas Lemos
- Jhayson Garcia Ramires Barbosa
- Giovanni Quilião Bernal
- Caio Gabriel Canedo Mariano

Professor orientador: Vitor Gabriel de Souza Farias.

## Licença

Trabalho acadêmico. Defina uma licença antes de publicar o repositório (MIT é uma opção comum). Enquanto isso não for feito, o código não tem licença de reuso.
