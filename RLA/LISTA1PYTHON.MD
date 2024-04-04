# Função para calcular o reajuste salarial
def calReajuste(sal, prof):
    # Realiza a seleção do reajuste salarial de acordo com a profissão
    if prof == "Técnico":
        # Aplica o reajuste de 50% sobre o salário atual
        sal_reaj = 1.5 * sal
    elif prof == "Gerente":
        # Aplica o reajuste de 30% sobre o salário atual
        sal_reaj = 1.3 * sal
    else:
        # Aplica o reajuste de 10% sobre o salário atual
        sal_reaj = 1.1 * sal
    
    # Retorna o salário reajustado
    return sal_reaj

# Função principal
def main():
    # Solicita ao usuário que digite o salário e a profissão
    print("Digite o salário e a profissão:")
    # Lê o salário e a profissão inseridos pelo usuário
    sal, prof = input().split()
    # Converte o salário para float
    sal = float(sal)

    # Calcula o salário reajustado
    sal_reaj = calReajuste(sal, prof)

    # Exibe o salário reajustado
    print("Salário Reajustado =", sal_reaj)

# Chama a função principal
if __name__ == "__main__":
    main()
