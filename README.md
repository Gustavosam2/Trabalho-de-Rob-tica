# Trabalho-de-Rob-tica
1.#include <iostream>
using namespace std;

int main() {
    // Declarando e inicializando variáveis de tipos primitivos do C++
    int inteiro = 10;              // Tipo inteiro
    char caractere = 'A';          // Tipo caractere
    float numeroFloat = 3.14f;     // Tipo float (precisão simples)
    double numeroDouble = 3.14159; // Tipo double (precisão dupla)
    bool booleano = true;          // Tipo booleano (true ou false)
    short numeroShort = 100;       // Tipo short (inteiro curto)
    long numeroLong = 100000L;     // Tipo long (inteiro longo)

    // Exibindo os valores das variáveis
    cout << "Valor do inteiro: " << inteiro << endl;
    cout << "Valor do caractere: " << caractere << endl;
    cout << "Valor do float: " << numeroFloat << endl;
    cout << "Valor do double: " << numeroDouble << endl;
    cout << "Valor do booleano: " << booleano << endl;
    cout << "Valor do short: " << numeroShort << endl;
    cout << "Valor do long: " << numeroLong << endl;

    return 0;
}

2#include <iostream>
using namespace std;

int main() {
    int num1, num2;

    // Leitura dos números
    cout << "Digite o primeiro número inteiro: ";
    cin >> num1;

    cout << "Digite o segundo número inteiro: ";
    cin >> num2;

    // Operações básicas
    int soma = num1 + num2;
    int subtracao = num1 - num2;
    int multiplicacao = num1 * num2;

    cout << "\nResultados:" << endl;
    cout << "Soma: " << soma << endl;
    cout << "Subtracao: " << subtracao << endl;
    cout << "Multiplicacao: " << multiplicacao << endl;

    // Verificação da divisão por zero
    if (num2 != 0) {
        float divisao = static_cast<float>(num1) / num2;
        cout << "Divisao: " << divisao << endl;
    } else {
        cout << "Divisao: Indefinida (divisao por zero)" << endl;
    }

    return 0;
}

3#include <iostream>
using namespace std;

int main() {
    // Declaração de Constantes e variáveis
    const float PI = 3.14159;  
    float raio, area;

    // Entrada do raio
    cout << "Digite o raio do círculo: ";
    cin >> raio;

    // Cálculo da área
    area = PI * raio * raio;

    // Exibição do resultado
    cout << "A área do círculo é: " << area << endl;

    return 0;
}

4. #include <iostream>
using namespace std;

int main() {
    // Declaração de variáveis
    int inteiro1 = 7, inteiro2 = 2;
    float flutuante1 = 7.0f, flutuante2 = 2.0f;
    double duplo1 = 7.0, duplo2 = 2.0;

    // Operações com int (sem casas decimais, resultado truncado)
    int resultado_int = inteiro1 / inteiro2;
    cout << "Divisão (int): 7 / 2 = " << resultado_int << " (truncado, sem casas decimais)" << endl;

    // Operações com float (com menos precisão)
    float resultado_float = flutuante1 / flutuante2;
    cout << "Divisão (float): 7.0 / 2.0 = " << resultado_float << " (com menos precisão)" << endl;

    // Operações com double (maior precisão)
    double resultado_double = duplo1 / duplo2;
    cout << "Divisão (double): 7.0 / 2.0 = " << resultado_double << " (mais preciso)" << endl;

    // Multiplicação exemplo adicional
    float multiplicacao_float = flutuante1 * flutuante2;
    double multiplicacao_double = duplo1 * duplo2;

    cout << "Multiplicação (float): 7.0 * 2.0 = " << multiplicacao_float << endl;
    cout << "Multiplicação (double): 7.0 * 2.0 = " << multiplicacao_double << endl;

    return 0;
}

5. #include <iostream>
#include <string>  // Necessária para usar std::string
using namespace std;

int main() {
    string nome;
    int idade;

    // Entrada de dados
    cout << "Digite seu nome: ";
    getline(cin, nome);  // Lê a linha inteira (inclui espaços)

    cout << "Digite sua idade: ";
    cin >> idade;

    // Mensagem personalizada
    cout << "\nOlá, " << nome << "! Você tem " << idade << " anos." << endl;

    return 0;
}

6. #include <iostream>
using namespace std;

// Função que recebe dois inteiros e retorna a soma
int soma(int a, int b) {
    return a + b;
}

int main() {
    int num1, num2;

    // Leitura dos números
    cout << "Digite o primeiro número: ";
    cin >> num1;

    cout << "Digite o segundo número: ";
    cin >> num2;

    // Chamada da função soma()
    int resultado = soma(num1, num2);

    // Exibição do resultado
    cout << "A soma é: " << resultado << endl;

    return 0;
}

7. #include <iostream>
using namespace std;

bool ehPar(int numero) {
    return numero % 2 == 0;
}

int main() {
    int n;
    cout << "Digite um número: ";
    cin >> n;

    if (ehPar(n)) {
        cout << "O número é par." << endl;
    } else {
        cout << "O número é ímpar." << endl;
    }

    return 0;
}

8. #include <iostream>
using namespace std;

// Função que exibe uma saudação
void mostrarMensagem() {
    cout << "Olá! Seja bem-vindo ao programa!" << endl;
}

int main() {
    // Chama a função para exibir a mensagem
    mostrarMensagem();
    return 0;
}

9. #include <iostream>
using namespace std;

// Função que retorna o quadrado de um número
int quadrado(int numero) {
    return numero * numero;
}

int main() {
    int n;
    cout << "Digite um número: ";
    cin >> n;

    cout << "O quadrado de " << n << " é " << quadrado(n) << endl;

    return 0;
}

10. #include <iostream>
using namespace std;

// Função que retorna o maior entre dois números float
float maior(float a, float b) {
    return (a > b) ? a : b;
}

int main() {
    float num1, num2;
    cout << "Digite dois números: ";
    cin >> num1 >> num2;

    cout << "O maior número é: " << maior(num1, num2) << endl;

    return 0;
}

11. #include <iostream>
using namespace std;

int main() {
    int valor = 42;           // Variável inteira
    int* ponteiro = &valor;   // Ponteiro apontando para a variável

    // Exibindo o valor da variável através do ponteiro
    cout << "Valor da variável: " << *ponteiro << endl;

    // Exibindo o endereço da variável
    cout << "Endereço da variável: " << ponteiro << endl;

    return 0;
}

12. #include <iostream>
using namespace std;

// Função que dobra o valor apontado
void dobrar(int* ptr) {
    *ptr = (*ptr) * 2;
}

int main() {
    int valor = 10;
    
    cout << "Antes: " << valor << endl;
    
    dobrar(&valor);  // Passa o endereço da variável para a função
    
    cout << "Depois: " << valor << endl;

    return 0;
}

13. #include <iostream>
using namespace std;

// Função que troca os valores de duas variáveis usando ponteiros
void trocar(int* a, int* b) {
    int temp = *a;
    *a = *b;
    *b = temp;
}

int main() {
    int x = 5, y = 10;

    cout << "Antes da troca:" << endl;
    cout << "x = " << x << ", y = " << y << endl;

    trocar(&x, &y); // Passa os endereços das variáveis

    cout << "Depois da troca:" << endl;
    cout << "x = " << x << ", y = " << y << endl;

    return 0;
}

14. #include <iostream>
using namespace std;

// Função que exibe os elementos de um vetor usando ponteiros
void exibirVetor(int* vet, int tamanho) {
    for (int i = 0; i < tamanho; i++) {
        cout << "Elemento " << i << ": " << *(vet + i) << endl;
    }
}

int main() {
    int numeros[5] = {10, 20, 30, 40, 50};

    exibirVetor(numeros, 5);  // Passa o vetor e o tamanho para a função

    return 0;
}

15. #include <iostream>
using namespace std;

int main() {
    float nota;
    float* pNota = &nota;

    cout << "Digite a nota do aluno: ";
    cin >> *pNota;  // Lê a nota usando o ponteiro

    if (*pNota >= 7.0) {
        cout << "Aluno aprovado!" << endl;
    } else {
        cout << "Aluno reprovado." << endl;
    }

    return 0;
}

16. #include <iostream>
using namespace std;

// Função que troca os valores usando referência
void trocar(int &a, int &b) {
    int temp = a;
    a = b;
    b = temp;
}

int main() {
    int x = 5, y = 10;

    cout << "Antes da troca: x = " << x << ", y = " << y << endl;

    trocar(x, y);  // Passagem por referência

    cout << "Depois da troca: x = " << x << ", y = " << y << endl;

    return 0;
}

17.  #include <iostream>
using namespace std;

// Função que altera os dois números
void alterar(int valor, int &referencia) {
    valor = valor + 10;         // Altera apenas localmente (por valor)
    referencia = referencia + 10; // Altera de verdade (por referência)

    cout << "Dentro da função - valor (por valor): " << valor << endl;
    cout << "Dentro da função - referencia (por referência): " << referencia << endl;
}

int main() {
    int a = 5, b = 5;

    cout << "Antes da função - a: " << a << ", b: " << b << endl;

    alterar(a, b);

    cout << "Depois da função - a: " << a << " (não muda)" << endl;
    cout << "Depois da função - b: " << b << " (foi alterado)" << endl;

    return 0;
}

18.  #include <iostream>
using namespace std;

// Função que incrementa o valor apontado por p
void incrementar(int* p) {
    (*p)++;  // Incrementa o valor apontado
}

int main() {
    int x = 10;
    cout << "Antes: x = " << x << endl;

    incrementar(&x);  // Passa o endereço de x

    cout << "Depois: x = " << x << endl;

    return 0;
}

19.  #include <iostream>
using namespace std;

// Função que calcula a média de três notas
float calcularMedia(float n1, float n2, float n3) {
    return (n1 + n2 + n3) / 3;
}

int main() {
    float nota1, nota2, nota3;

    cout << "Digite a primeira nota: ";
    cin >> nota1;

    cout << "Digite a segunda nota: ";
    cin >> nota2;

    cout << "Digite a terceira nota: ";
    cin >> nota3;

    float media = calcularMedia(nota1, nota2, nota3);

    cout << "A média das notas é: " << media << endl;

    return 0;
}

20.  #include <iostream>
#include <string>
using namespace std;

// Função que exibe a situação do aluno
void verificarSituacao(string nome, float nota) {
    cout << "Aluno: " << nome << endl;
    cout << "Nota: " << nota << endl;

    if (nota >= 7.0) {
        cout << "Situação: Aprovado" << endl;
    } else {
        cout << "Situação: Reprovado" << endl;
    }
}

int main() {
    string nomeAluno;
    float notaAluno;

    cout << "Digite o nome do aluno: ";
    getline(cin, nomeAluno);

    cout << "Digite a nota do aluno: ";
    cin >> notaAluno;

    verificarSituacao(nomeAluno, notaAluno);

    return 0;
}

21.  #include <iostream>
using namespace std;

// Função que calcula a área do retângulo
float calcularAreaRetangulo(float base, float altura) {
    return base * altura;
}

int main() {
    float b, h;

    cout << "Digite a base do retângulo: ";
    cin >> b;

    cout << "Digite a altura do retângulo: ";
    cin >> h;

    float area = calcularAreaRetangulo(b, h);

    cout << "A área do retângulo é: " << area << endl;

    return 0;
}

22.  #include <iostream>
using namespace std;

int main() {
    const float BONUS = 500.0;  // Bônus fixo definido com const
    float salario;

    cout << "Digite o salário: ";
    cin >> salario;

    float total = salario + BONUS;

    cout << "Salário com bônus: " << total << endl;

    return 0;
}

23.  #include <iostream>
#ifndef FUNCOES_H
#define FUNCOES_H

int main() {
// Declaração da função mostrarInfo
void mostrarInfo();
#endif // FUNCOES_H
    return 0;
}

24. #include <iostream>
// Função que calcula a média dos elementos de um vetor
double calcularMedia(int* vetor, int tamanho) {
    double soma = 0.0;
    for (int i = 0; i < tamanho; ++i) {
        soma += vetor[i];
    }
    return soma / tamanho;
}
int main() {
    // Criação de um vetor de 10 elementos
    int vetor[10] = {10, 20, 30, 40, 50, 60, 70, 80, 90, 100};
    // Chamada da função para calcular a média
    double media = calcularMedia(vetor, 10);
    // Exibição do resultado
    std::cout << "A média dos elementos do vetor é: " << media << std::endl;
    return 0;
}

25. #include <iostream>
// Função que inverte o sinal de uma variável
void inverterSinal(int &valor) {
    valor = -valor; // Inverte o sinal
}
int main() {
    int numero;
    // Solicita ao usuário para inserir um número
    std::cout << "Digite um número: ";
    std::cin >> numero;
    // Exibe o valor original
    std::cout << "Valor original: " << numero << std::endl;
    // Chama a função para inverter o sinal
    inverterSinal(numero);
    // Exibe o valor após inverter o sinal
    std::cout << "Valor após inverter o sinal: " << numero << std::endl;
    return 0;
}

26. #include <iostream>
    using namespace std;
// Protótipos das funções
void menu();
void calcularSoma();
void calcularSubtracao();
void calcularMultiplicacao();
int main() {
    menu(); // Chama o menu principal
    return 0;
}
void menu() {
    int opcao;
    
    do {
    cout << "\n=== MENU DE CALCULOS ===" << endl;
    cout << "1. Soma" << endl;
    cout << "2. Subtracao" << endl;
    cout << "3. Multiplicacao" << endl;
    cout << "0. Sair" << endl;
    cout << "Escolha uma opcao: ";
    cin >> opcao;
    switch(opcao) {
    case 1:
    calcularSoma();
    break;
    case 2:
    calcularSubtracao();
    break;
    case 3:
    calcularMultiplicacao();
    break;
    case 0:
    cout << "Saindo do programa..." << endl;
    break;
    default:
    cout << "Opcao invalida!" << endl;
        }
    } while(opcao != 0);
}
void calcularSoma() {
    float a, b;
    cout << "Digite dois numeros para somar: ";
    cin >> a >> b;
    cout << "Resultado: " << a + b << endl;
}
void calcularSubtracao() {
    float a, b;
    cout << "Digite dois numeros para subtrair: ";
    cin >> a >> b;
    cout << "Resultado: " << a - b << endl;
}
void calcularMultiplicacao() {
    float a, b;
    cout << "Digite dois numeros para multiplicar: ";
    cin >> a >> b;
    cout << "Resultado: " << a * b << endl;
}

28. #include <iostream>
#include <string>
using namespace std;
struct Pessoa {
    string nome;
    int idade;
    float altura; 
};
void imprimirDados(Pessoa* p) {
    cout << "\nDADOS PESSOAIS:" << endl;
    cout << "Nome: " << p->nome << endl;
    cout << "Idade: " << p->idade << " anos" << endl; 
    cout << "Altura: " << p->altura << " metros\n" << endl;
}
int main() {
    // Variáveis para armazenar os dados
    string nome_pessoa;
    int idade_pessoa;
    float altura_pessoa;
    // Solicita os dados ao usuário
    cout << "Digite o nome: ";
    getline(cin, nome_pessoa);
    
    cout << "Digite a idade: ";
    cin >> idade_pessoa;
    
    cout << "Digite a altura (em metros): ";
    cin >> altura_pessoa;
    // Cria e preenche a estrutura
    Pessoa pessoa;
    pessoa.nome = nome_pessoa;
    pessoa.idade = idade_pessoa;
    pessoa.altura = altura_pessoa;
    // Imprime os dados passando o ponteiro
    imprimirDados(&pessoa);
    return 0;
}

29. #include <iostream>
using namespace std;
// Função template para trocar valores usando ponteiros
template <typename T>
void trocarValores(T* ptr1, T* ptr2) {
    T temp = *ptr1;  // Armazena o valor do primeiro ponteiro
    *ptr1 = *ptr2;   // Atribui o valor do segundo ponteiro ao primeiro
    *ptr2 = temp;    // Atribui o valor temporário ao segundo ponteiro
}
int main() {
    // Demonstração com inteiros
    int a = 10, b = 20;
    cout << "Antes da troca (int): a = " << a << ", b = " << b << endl;
    trocarValores(&a, &b);
    cout << "Depois da troca (int): a = " << a << ", b = " << b << endl << endl;
    // Demonstração com floats
    float x = 3.14f, y = 2.71f;
    cout << "Antes da troca (float): x = " << x << ", y = " << y << endl;
    trocarValores(&x, &y);
    cout << "Depois da troca (float): x = " << x << ", y = " << y << endl << endl;
    return 0;
}

30. #include <iostream>

#include "funcoes.h"
using namespace std;
int main() {
    int num = 5;
    
    cout << "\n=== Demonstracao de Passagem de Parametros ===" << endl;
    cout << "Valor original: " << num << endl;
    
    // 1. Passagem por valor
    passagemPorValor(num);
    cout << "Apos passagemPorValor: " << num << endl; // Não altera o original
    
    // 2. Passagem por referência
    passagemPorReferencia(num);
    cout << "Apos passagemPorReferencia: " << num << endl; // Altera o original
    
    // Reinicia o valor para próxima demonstração
    num = 5;
    
    // 3. Passagem por ponteiro
    passagemPorPonteiro(&num);
    cout << "Apos passagemPorPonteiro: " << num << endl; // Altera o original
    
    return 0;
}
