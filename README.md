# GFT-Algorismo-Romanos
GFT-START#5 2022


//Exercício 1

 programa
{
	funcao inicio() 
	{
	    
	   inteiro valorDiaria, diasHospedagem
	   
	   escreva("digite o valor da diaria do hotel:")
	   leia(valorDiaria)
	   escreva("digite a quantidade de dias da hospedagem:")
	   leia(diasHospedagem)
	   
	   enquanto(diasHospedagem < 0 ou diasHospedagem > 4000 ou valorDiaria < 0){
	       escreva("valor invÃ¡lido, digite novamente: \n")
	       escreva("diaria:")
	       leia(valorDiaria)
	       escreva("hospedagem:")
	       leia(diasHospedagem)
	       
	   }
	escreva("Fim do Programa!")
	
	}
}

//exercício2

//exercício3

programa {
    funcao inicio() {
        // Declaramos uma variável e essa já vai ser endereçada na memória do nosso computador
        inteiro x = 10
        escreva("\nO valor atual de x é " + x)
        
        // Realizaremos a operação de somar
        somar(x)
        
        escreva("\nO valor atual de x é " + x)
    }
    
    // Para dizermos que o parâmetro será passado por referencia, usamos o caracter & antes no nome da variável
    funcao somar(inteiro &x)
    {
        /* 
            Aqui, estamos pegando o valor atual do numeroParaSomar e somando com 10
            Então, se tivermos 10 no valor atual, teremos 10 + 10
            O resultado dessa soma será o novo valor da variável numeroParaSomar
        */
        x = x + 10
    }
}
                    

//exercício 4

programa 
{
	funcao inicio() 
	{
	    real classeVip, totalDias = 0.0 
	    cadeia nome, sinal     = "continua"
	    inteiro idade          = 0, gratuito = 0, meia = 0
	    
	    
	    escreva("qual o valor da classeVip, \n")
	    leia(classeVip)
	    
	    enquanto(sinal!= "s" e sinal!= "n")
	    {
	    escreva("qual o nome do cliente,\n")
	    leia(nome)
	    escreva("qual a idade maior ou idade menor,\n")
	    leia(idade)
	    escreva("para continuar registrando cliente digite continua,ex:[s] ou [n],\n")
	    se(idade<4)
	    {
	        escreva(nome,"possui gratuidade,\n")
	        gratuito++
	        escreva("para continuar registrando cliente digite continua,ex:[s] ou [n],\n")
	        leia(sinal)
	        limpa()
	    }
	    senao se(idade>80)
	    {
	        totalDias=totalDias+0.5*classeVip
	        escreva(nome,"paga meia,\n")
	        meia++
	        escreva("para continuar registrando cliente digite continuar,ex:[s] ou [n] ,\n")
	        leia(sinal)
	        limpa()
	   }
	   
	   
	    }
	    escreva("o total do cliente é:R$",totalDias,";",gratuito,"gratuidade(s);",meia,"meia(s)")
	    
		
	}
}
