# Opções do suporte 
duvidas = {
    "1": "Diretrizes e Politica",
    "2": "F.A.Q.",
    "3": "Fale Conosco",
    "4": "Sair?",
}

# Base de dados para cada opção
duvidas_x = {
    "1": "Diretrizes",
    "2": "Politica",
    "3": "Manual de Integracao",
    "4": "Exit",
}

duvidas_y = {
    "1": "Informacoes",
    "2": "Beneficios",
    "3": "Meus Deveres",
    "4": "Exit",
}

duvidas_z = {
    "1": "Endereco/Telefone",
    "2": "Website",
    "3": "Intranet do colaborador",
    "4": "Exit",
}

# função para mostrar as opções de atendimento e capturar a escolha do usuário
def escolher_opcao():
    print("Para atendimento pfv digite o numero correspondente e clique Enter:")
    for selecione, pergunta in duvidas.items():
        print(f"{selecione}. {pergunta}")
    escolha = input("Opcao escolhida : ")
    return escolha

# função para mostrar as perguntas e respostas correspondentes à opção escolhida
def mostrar_perguntas_respostas(escolha):
    if escolha == "1":
        perguntas_respostas = duvidas_x
    elif escolha == "2":
        perguntas_respostas = duvidas_y
    elif escolha == "3":
        perguntas_respostas = duvidas_z
    elif escolha == "4":
        exit()
    else:
        print("Opção inválida, tente novamente!")
    
        return
    
    print("Selecione um Topico:")
    for pergunta in perguntas_respostas.values():
        print(pergunta)
    selecione = input("Pergunta escolhida: ")
    resposta = perguntas_respostas.get(escolha)
    if resposta:
        print(f"Resposta: {resposta}")
    else:
        print("Tente Novamente/Try Again !")
    
# loop principal do bot
while True:
    selecione = escolher_opcao()
    mostrar_perguntas_respostas(selecione)
    reiniciar = input("Deseja reiniciar este atendimento? (s/n) ")
    if reiniciar.lower() != "s":
        break
