# Estudos-de-base-de-programa-o
Objetivo de escrever os codigos que serao usados de base para o aprendizado de programação

##############################################################
####################   PROGRAMA 1  ###########################
###    Simei Tarse Sobrinho Santos                         ###
###  OBJETIVO: CRIAR JANELA FUNCIONAL COM BOTAO            ###
###                                                        ###
###---------------------ETAPAS-----------------------------###
### 1 - Importar biblioteca                                ###
### 2 - Criar a função que o botao vai acionar             ###
### 3 - Criar janela principal                             ###
### 4 - Criar botao funcional                              ###
### 5 - Posicionar o botao na janela e iniciar             ###
###                                                        ###
##############################################################
##############################################################

#importar bibliotecas
import tkinter as tk

#criar função que o botão vai acionar
def clique_botao():
    print("O botão foi clicado!")

#criar a janela principal
janela = tk.Tk()
janela.title("Simei Tarse")
janela.geometry("300x200")

#Criar o botão funcional (o termo "command" lincado a 
#função "def clique_botao():") faz o botao funcionar
botao = tk.Button(janela, text="clicar", command=clique_botao)

#posicionar o botao
botao.pack(pady=50)
janela.mainloop()
