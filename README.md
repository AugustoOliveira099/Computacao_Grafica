# Computação gráfica
Disciplina cursada na UFRN durante a graduação de engenharia de computação e que estuda as diferentes técnicas de computação gráfica existentes.

## Projeto
Grupo:
- Diego de Oliveira;
- João Gabriel;
- José Augusto;
  
A ideia do projeto foi representar um eclipse solar, tendo o sol (objeto fonte de luz) e a lua translacionando a Terra. Serão utilizadas duas câmeras de visualização, estando uma no espaço para que seja possível visualizar o movimento da lua em torno da Terra. A câmera terrestre observará como uma pessoa, sendo possível visualizar o anel de fogo.

## Uso
Para utilizar, certifique-se de ter OpenGL instalado. 

No Linux (creio que em qualquer sistema operaciona do tipo unix funcione), basta executar o comando a seguir, no terminal, dentro do diretório do projeto:
```
gcc -o eclipse eclipse.c -lm -lGL -lGLU -lglut
```

Em seguida, execute o arquivo executável criado:
```
./eclipse
```

No windows, utilizei a IDE "Dev C++" e adicionei os devidos arquivos para que o OpenGL e o Glut funcionassem, seguindo este [tutorial](https://www.youtube.com/watch?app=desktop&v=bbAdDusjGVA&ab_channel=Jogos%26Programa%C3%A7%C3%A3o).

## Comandos
Os comandos disponíveis na aplicação são:
- W/w: Aproxima a câmera;
- S/s: Afasta a imagem;
- A/a: Move a câmera para esquerda;
- D/d: Moce a câmera para direita;
- Q/q: Rotaziona a câmera para esquerda  em torno da Terra;
- E/e: Rotaziona a câmera para direita em torno da Terra;
- F/f: Rotaziona a câmera para cima em torno da Terra;
- V/v: Rotaziona a câmera para baixo em torno da Terra;
- M/m: Interrompe/reinicia a rotação da Lua;
- Botão esquerdo do mouse: Move a lua com um movimento contrário à sua rotação (cada clique move um pouco, melhor vizualizado com a lua parada);
- Botão direito do mouse: Move a lua com um movimento a favor da sua rotação (cada clique move um pouco, melhor vizualizado com a lua parada);
- Scroll do mouse: No Linux faz a mesma coisa que o W/w e o S/s (no windows não funcionou).

![Gif da aplicação em execução](assets/eclipse.gif)
