# Swift Fundamentals II

**Tuplas, Arrays e Dicionários**

  

     /
    /: Playground - noun: a place where people can play
    
    import UIKit
    
    //========================================================
    
    // TUPLAS (TUPLES)
    
    //========================================================
    
    // Exemplo de declaração com valores de um mesmo tipo:
    
    var empresa = ("Apple", "iOS", "Swift")
    
    // Se decompormos essa tupla, ela ficaria da seguinte maneira:
    
    //empresa: (String, String, String) = { 0 = "Apple",
    
    // 1 = "iOS",
    
    // 2 = "Swift"
    
    //}
    
    //Declaração com valores de tipos diferentes:
    
    var pessoa = ("Pedro Alvares Cabral", 40, 87.3)
    
    // Ao decompormos essa tupla, temos o seguinte resultado:
    
    //pessoa: (String, Int, Double) = { 0 = "Pedro Alvares Cabral"
    
    // 1=40
    
    // 2 = 87.300000000000
    
    //}
    
    print(empresa.0)
    
    print(empresa.2)
    
    //--------------------------------------
    
    var ferrariEnzo = (cilindros: "V12", potencia: 660)
    
    print (ferrariEnzo.potencia)
    
    var (x, y) = ferrariEnzo
    
    // A variável x irá receber o valor de cilindros e y o valor de potência.
    
    // Ignorar um elemento da tupl, colocar underscore (_)
    
    var (a, _) = ferrariEnzo
    
    //========================================================
    
    // ARRAYS
    
    //========================================================
    
    // Sintaxe de declaração de forma explícita e vazio:
    
    var arrayVazio = [String]()
    
    // Array com tipagem explícita e com dados:
    
    var arrayComTipagemExplicita : [String] = ["valor1", "valor2", "valor3", "valor4"]
    
    // Array com tipagem implícita e com dados:
    
    var arrayComTipagemImplicita = ["valor1", "valor2", "valor3", "valor4"]
    
    // Adicionar valores
    
    var arrayItens = [String]()
    
    arrayItens.append("PrimeiroValor")
    
    arrayItens.append("SegundoValor")
    
    arrayItens += ["ValorAdicionadoSemAppend"]
    
    arrayItens.insert("Adicionado em índice específico", at: 2)
    
    // Remoção de Itens
    
    arrayItens.remove(at: 1)
    
    // Substitição de Itens
    
    arrayItens[0] = "valor substituído"
    
    //========================================================
    
    // DICIONÁRIOS (DICTIONARYS)
    
    //========================================================
    
    //Sintaxe de declaração de forma explícita e vazio
    
    var dicionarioItens = [String : Int]()
    
    //Dicionário com tipagem explícita e com dados:
    
    var dicionarioItens : [String : Int] = ["chave1": 1, "chave2": 2]
    
    //Dicionário com tipagem implícita e com dados:
    
    var dicionarioItens = ["chave1": 1, "chave2": 2]
    
    dicionarioItens [“chave1”] = 1
    
    dicionarioItens [“chave2”] = 2
    
    dicionarioItens [“chave3”] = 3
    
    dicionarioItens.removeValue(forKey: "chave1")
