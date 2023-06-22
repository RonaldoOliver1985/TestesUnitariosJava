# TestesUnitariosJava

<p>
  Certamente! Vou mostrar um exemplo simples de como criar testes unitários em Java usando a biblioteca JUnit. Suponha que você tenha uma classe chamada "Calculadora" com dois métodos: "somar" e "subtrair". Vamos criar testes para esses métodos.

Passo 1: Configurar o ambiente
Certifique-se de ter o JUnit configurado no seu projeto. Você pode adicionar a dependência do JUnit no arquivo pom.xml (se estiver usando Maven) ou importar o JUnit no seu projeto, caso esteja usando outra forma de gerenciamento de dependências.

Passo 2: Criar a classe de teste
Crie uma nova classe chamada "CalculadoraTest" e adicione a anotação @Test da biblioteca JUnit antes de cada método de teste.
</p>

import org.junit.jupiter.api.Test;
import static org.junit.jupiter.api.Assertions.*;

public class CalculadoraTest {
    
    @Test
    public void testSomar() {
        Calculadora calc = new Calculadora();
        int resultado = calc.somar(3, 5);
        assertEquals(8, resultado);
    }

    @Test
    public void testSubtrair() {
        Calculadora calc = new Calculadora();
        int resultado = calc.subtrair(10, 4);
        assertEquals(6, resultado);
    }
}

</br>
<p>
  Passo 3: Escrever os testes
Dentro de cada método de teste, você pode criar uma instância da classe "Calculadora" e chamar os métodos que deseja testar. Em seguida, use os métodos de asserção fornecidos pela biblioteca JUnit, como o assertEquals, para verificar se o resultado é o esperado.

Passo 4: Executar os testes
Execute os testes unitários clicando com o botão direito na classe de teste (no Eclipse ou IntelliJ, por exemplo) e selecionando "Run as" -> "JUnit test". Você também pode executar os testes usando ferramentas de linha de comando ou integração contínua.

Os testes unitários ajudam a garantir que suas classes e métodos funcionem corretamente e fornecem uma maneira de verificar se as alterações no código introduzem regressões.
</p>
