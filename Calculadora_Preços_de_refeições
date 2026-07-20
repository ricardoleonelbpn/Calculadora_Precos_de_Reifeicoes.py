# Adicionei ao código a parte de sobremesa e bebida, e o cálculo do total da refeição com esses valores.
# Adicionei também a solicitação do anunciado da tarefa para me direcionar na criação dos códigos.
# Adicionei a parte de desconto e troco, que não estava no código original, para que o codigo fique mais descritivo.
# Para finalizar adicionei um resumo da refeição, com todos os valores calculados, para que o usuário tenha uma visão geral do que foi gasto, simulando um recibo de compra.
"""
O preço da refeição de uma criança (ponto flutuante).
O preço da refeição de um adulto (ponto flutuante).
O número de crianças (inteiro).
O número de adultos (inteiro).
O preço da sobremesa (ponto flutuante).
O preço da bebida (ponto flutuante).
"""

preço_refeição_criança = float(input("Digite o preço da refeição de uma criança? "))
preço_refeição_adulto = float(input("Digite o preço da refeição de um adulto? "))
número_crianças = int(input("Digite o número de crianças? "))
número_adultos = int(input("Digite o número de adultos? "))
preço_sobremesa = float(input("Digite o preço da sobremesa? "))
preço_bebida = float(input("Digite o preço da bebida? "))
quantidade_da_sobremesa = int(input("Quantas sobremesas foram compradas? "))
quantidade_da_bebida = int(input("Quantas bebidas foram compradas? "))

"""
Determine o subtotal da refeição (antes de adicionar o imposto sobre vendas) 
multiplicando o número de crianças pelo preço da refeição e multiplicando o número de adultos pelo preço da refeição e somando esses dois valores.
Exiba o subtotal.
"""
subtotal_refeição = (preço_refeição_criança * número_crianças) + (preço_refeição_adulto * número_adultos)
subtotal_sobremesa = preço_sobremesa * quantidade_da_sobremesa
subtotal_bebida = preço_bebida * quantidade_da_bebida
subtotal = subtotal_refeição + subtotal_sobremesa + subtotal_bebida
print(f"\nO subtotal da refeição é: R$ {subtotal:.2f}")

"""
Peça ao usuário a taxa de imposto sobre vendas em porcentagem (ponto flutuante). 
Observe que essa porcentagem deve ser inserida e armazenada como um número como 6 ou 6.5, e não 0.06 ou 0.065.
Calcule e exiba o imposto sobre vendas multiplicando o subtotal pela taxa de imposto sobre vendas dividida por 100.
Calcule e exiba o preço total da refeição adicionando o subtotal e o imposto sobre vendas.
"""

imposto_sobre_vendas = float(input("\nQual é a taxa de imposto sobre vendas em porcentagem: "))
calculo_imposto = subtotal * (imposto_sobre_vendas / 100)
print(f"O imposto sobre vendas é: R$ {calculo_imposto:.2f}")
total_refeição = subtotal + calculo_imposto
print(f"O preço total da refeição é: R$ {total_refeição:.2f}")

"""
Peça ao usuário a porcentagem de desconto (ponto flutuante).
Calcule e exiba o valor do desconto multiplicando o preço total da refeição pela porcentagem de desconto dividida por 100.
Calcule e exiba o preço total da refeição com desconto subtraindo o valor do desconto do preço total da refeição.
"""
desconto = float(input("\nQual é a porcentagem de desconto: "))
valor_desconto = total_refeição * (desconto / 100)
total_refeição_com_desconto = total_refeição - valor_desconto
print(f"O valor do desconto é: R$ {valor_desconto:.2f}")
print(f"O preço total da refeição com desconto é: R$ {total_refeição_com_desconto:.2f}")

"""
Peça ao usuário o valor do pagamento (ponto flutuante).
Calcule e exiba a mudança.
"""

pagamento = input("\nQual é o valor do pagamento: ")
pagamento = pagamento.replace(",", ".")
pagamento = float(pagamento)
troco = pagamento - total_refeição_com_desconto
print(f"Seu troco é: R$ {troco:.2f}")
print()

print("------------------------------------------------------------------------------------")
print("                        RESUMO DA REFEIÇÃO                              ")          
print(f"\nTotal da refeição: R$ {subtotal_refeição:.2f} ")
print(f"Total da sobremesa: R$ {subtotal_sobremesa:.2f} ")
print(f"Total da bebida: R$ {subtotal_bebida:.2f} ")
print(f"Valor do imposto sobre vendas: R$ {calculo_imposto:.2f} ")
print(f"Valor do desconto: R$ {valor_desconto:.2f} ")
print(f"Preço total da refeição com desconto: R$ {total_refeição_com_desconto:.2f} ")

print("\n------------------------------------------------------------------------------------")
print("                        OBRIGADO PELA PREFERÊNCIA!                              ")
print()


