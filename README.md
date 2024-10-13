Para rodar o simulador:

1.Prepare os arquivos:
automaton_diagram.json: O diagrama do autômato.
test_cases.txt: Os casos de teste.

2.Rodar o script:
Salve o código em um arquivo, por exemplo, automaton_simulator.js.
Execute o script com o Node.js:

node automaton_simulator.js

3.Verifique o arquivo de saída (output.txt), que contém os resultados dos testes.

Exemplo:

automaton_diagram.json:
{
  "initial": 0,
  "final": [0],
  "transitions": [
    { "from": 0, "read": "0", "to": 1 },
    { "from": 1, "read": "0", "to": 0 },
    { "from": 0, "read": "1", "to": 0 },
    { "from": 1, "read": "1", "to": 1 }
  ]
}

test_cases.txt:
0;1
1;0
00;1
01;0
10;0
110;1
1010;1

Saída (output.txt):

Entrada: "0"; Esperado: 1; Resultado: 1; Tempo: 0.001ms
Entrada: "1"; Esperado: 0; Resultado: 0; Tempo: 0.002ms
Entrada: "00"; Esperado: 1; Resultado: 
