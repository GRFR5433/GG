def for_te():
    print("Contagem de 0 a 1:")
    G=input("-")
    for G in range(2):
        print(G)

def while_true():
    print("Digite números (ou deixe em branco para parar):")
    while True:
        GG = input("> ")
        if GG == "":
            print("Saindo do loop.")
            break
        
        try:
            GG = int(GG)  
            if GG < 0:
                print("Por favor, digite um número positivo.")
            else:
               
                print(f"Contando de 0 até {GG}:")
                for i in range(GG + 1):
                    print(i)
                    
        except ValueError:
            print("Por favor, digite um número válido.")

               
while True:
    print("\n         -MENU-")    
    print("-" * 30)
    print("1 - for, 2 - While, 3 - Sair")
    opcoes = input("Digite uma OPÇÃO acima☝: ")  

    match opcoes:
        case '1':
            print("-" * 40)
            print("Resultado:")
            for_te()
            print("-" * 40)
        case '2':
            print("-" * 40)
            print("Resultado:")
            while_true()
            print("-" * 40)
        case '3':
            print("Saindo...")
            print("Adeus até mais tarde! 😑👍")
            break 
        case _:
            print("Opção inválida! Tente novamente.")

