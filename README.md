🏅 Projeto: Classe Atleta (JavaScript)
📖 Descrição

Este projeto implementa uma classe Atleta em JavaScript, responsável por armazenar e processar informações sobre um atleta, incluindo nome, idade, peso, altura e notas de desempenho.
A classe fornece métodos para calcular a categoria etária, o IMC (Índice de Massa Corporal) e a média válida das notas (desconsiderando a maior e a menor nota).

🧩 Estrutura da Classe

A classe Atleta possui os seguintes atributos:

nome → nome do atleta

idade → idade do atleta

peso → peso em quilogramas

altura → altura em metros

notas → array com notas numéricas

E os seguintes métodos:

Método	Descrição
calculaCategoria()	Define a categoria com base na idade
calculaIMC()	Calcula o IMC usando a fórmula peso / (altura²)
calculaMediaValida()	Calcula a média das notas, descartando a maior e a menor
obtemNomeAtleta()	Retorna o nome do atleta
obtemIdadeAtleta()	Retorna a idade do atleta
obtemPesoAtleta()	Retorna o peso do atleta
obtemNotasAtleta()	Retorna todas as notas do atleta
obtemCategoria()	Retorna a categoria do atleta
obtemIMC()	Retorna o IMC calculado
obtemMediaValida()	Retorna a média válida calculada
⚙️ Regras Utilizadas
1. Categorias
Idade	Categoria
9 a 11	Infantil
12 a 13	Juvenil



IMC = peso / (altura * altura)


const atleta = new Atleta("Cesar Abascal", 30, 80, 1.70, [10, 9.34, 8.42, 10, 7.88]);

atleta.calculaCategoria();
atleta.calculaIMC();
atleta.calculaMediaValida();

console.log(`Nome: ${atleta.obtemNomeAtleta()}`);
console.log(`Idade: ${atleta.obtemIdadeAtleta()}`);
console.log(`Peso: ${atleta.obtemPesoAtleta()}`);
console.log(`Altura: ${atleta.altura}`);
console.log(`Notas: ${atleta.obtemNotasAtleta()}`);
console.log(`Categoria: ${atleta.obtemCategoria()}`);
console.log(`IMC: ${atleta.obtemIMC()}`);
console.log(`Média válida: ${atleta.obtemMediaValida()}`);
14 a 15	Intermediário
16 a 30	Adulto
Outras idades	Sem categoria
