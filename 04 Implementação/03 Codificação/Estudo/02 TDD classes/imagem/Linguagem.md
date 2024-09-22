# Javascript (variáveis)

Javascript (variáveis)
let name = "leonardo"
let password = 123456
let email= "leo@gmail.com"
let value= false

# Java (variáveis)

Java (variáveis)
String name = "leonardo";
int password = 123456;
String email = "leo@gmail.com";
boolean value = false;

# Javascript (função)

// Função que soma dois números e retorna o resultado
function somar(a, b) {
return a + b;
}

# Java (método)(dentro da classe)\*

// Método que soma dois números e retorna o resultado
public int somar(int a, int b) {
return a + b;
}

# Javascript (classe)

class NameClasse {
variável: string;

// Construtor da classe
constructor(variável: string) {
this.variável
}

// Método da classe que retorna a variável
metodoClasse(): string{
return this.variável
}

};

# Java (classe)\*

public class NameClasse {
private String variavel;

// Construtor da classe
public NameClasse(String variavel) {
this.variavel = variavel;
}

// Método da classe que retorna a variável
public String metodoClasse() {
return this.variavel;
}

}

# Javascript (teste)

test('Deve criar uma classe no sistema', () => {
//Give(dado que - instâncias)
const variávelObjeto = new NameClasse(“parametro”)
//When (quando acontecer algo - método)
const variável = variávelObjeto.metodoClasse()
//then (Então faça isso - expect)
expect(variável).toBe('parametro')
})

# Java (teste)

public class NameClasseTest {
@Test
public void deveCriarUmaClasseNoSistema() {
// Given (dado que - instâncias)
NameClasse variavelObjeto = new NameClasse("parametro");
// When (quando acontecer algo - método)
String variavel = variavelObjeto.metodoClasse();
// Then (então faça isso - assertion)
assertEquals("parametro", variavel);
}
}
