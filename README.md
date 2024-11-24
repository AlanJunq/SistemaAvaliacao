# Sistema de Avaliação

Este programa calcula a média de um aluno com base nas notas das provas e do trabalho, e determina se o aluno foi aprovado ou reprovado.

## Como Usar

1. O programa solicita três entradas:
   - Nota da primeira prova.
   - Nota da segunda prova.
   - Nota do trabalho.

2. O programa calcula a média e exibe a situação do aluno:
   - **Aprovado** se a média for 6 ou superior.
   - **Reprovado** se a média for abaixo de 6.

## Como Executar

### Passos

1. **Crie um arquivo Java** com o código abaixo:

   ```java
   import javax.swing.JOptionPane;

   public class SistemaAvaliacao {
       public static void main(String[] args) {
           double notaProva1 = Double.parseDouble(JOptionPane.showInputDialog("Digite a nota da primeira prova:"));
           double notaProva2 = Double.parseDouble(JOptionPane.showInputDialog("Digite a nota da segunda prova:"));
           double notaTrabalho = Double.parseDouble(JOptionPane.showInputDialog("Digite a nota do trabalho:"));

           double media = (notaProva1 + notaProva2 + notaTrabalho) / 3;
           String situacao = (media >= 6) ? "Aprovado" : "Reprovado";

           JOptionPane.showMessageDialog(null, "Média: " + media + "\nSituação: " + situacao);
       }
   }

2. **Compile o código:**

javac SistemaAvaliacao.java

3. **Execute o programa:**

java SistemaAvaliacao

