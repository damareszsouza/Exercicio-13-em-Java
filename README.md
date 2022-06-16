# Exercicio-13-em-Java
Tipos Enumerados - Livro Cartilha Java


public class DayTripper {
 public enum Day { MON, TUE, WED, THU, FRI, SAT, SUN };
 public static void main(String[ ] args) {
 Day d -
 Day.MON;
 System.out.println("Initially d is "  d);
 d -
 Day.WED;
 System.out.println("Then it is "  d);
 Day t -
 Day.valueOf("WED");
 System.out.println("I say d and t are the same: "  (d -
-
 t));
 }
}
A saída deste programa é:
Initially d is MON
Then it is WED
I say d and t are the same: true

Tipos enumerados
Desde a versão SE 5, Java suporta tipos enumerados chamados de enums. Esses 
tipos são permitidos apenas para que se possa obter valores provenientes de con-
juntos específicos de nomes. Eles são declarados dentro de uma classe como segue:
 modificador enum nome {nome_valor0, nome_valor1, ..., nome_valorn–1}
onde o modificador pode ser vazio, public, protected ou private. O nome desta enu-
meração, nome, pode ser qualquer identificador Java. Cada um dos identificadores 
de valor, nome_valori
, é o nome de um possível valor que variáveis desse tipo podem 
assumir. Cada um desses nomes de valor pode ser qualquer identificador Java legal, 
mas, por convenção, normalmente eles começam por letra maiúscula. Por exemplo, 
a seguinte definição de tipo enumerado pode ser útil em um programa que deve lidar 
com datas:
 public enum Day { MON, TUE, WED, THU, FRI, SAT, SUN };
Uma vez definido, um tipo enumerado pode ser usado na definição de outras 
variáveis da mesma forma que um nome de classe. Entretanto, como o Java conhece 
todos os nomes dos valores possíveis para um tipo enumerado, se um tipo enumerado 
for usado em uma expressão string, o Java irá usar o nome do valor automaticamente. 
Tipos enumerados também possuem alguns métodos predefinidos, incluindo o méto-
do valueOf, que retorna o valor enumerado que é igual a uma determinada string. Um 
exemplo de uso de tipo enumerado pode ser visto no Trecho de Código.
