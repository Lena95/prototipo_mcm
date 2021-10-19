# prototipo_mcm

from tkinter import*
from tkinter.font import 

class Agradecimento(Toplevel): 
    cor_tela = '#3F7958' # verde
    cor_root = '#656D4A' # verde 
    cor_2 = '#E2E237' # amarelo 
    cor_fonte = '#000000' # preto 
    cor_botao = '#FFFFFF' # branco 

    def __init__(self, original): 
        self.frame_original = original
        self.frame_original = original 
        Toplevel.__init__(self)
        self.geometry('375x600+975+10')
        self.configure(bg = self.cor_botao)
        self.title("MCM GÁS")
        self.widgets()
        self.frames()

    def widgets(self):
        label_mcm=Label(self, text="MCM GÁS", bg=self.cor_botao, font=("Broadway", 22))  
        label_mcm.place(relx=0, rely=0, relheight=0.20, relwidth=1.0)

        label_pedidoFeito=Label(self, text="SEU PEDIDO JÁ FOI FEITO!", fg=self.cor_tela, bg=self.cor_botao, font=("Times New Roman", 10))
        label_pedidoFeito.place(relx=0.15, rely=0.17, relheight=0.10, relwidth=0.73)

        label_agradecimento=Label(self, text="AGRADECEMOS SUA PREFERÊNCIA!", fg=self.cor_tela, bg=self.cor_botao, font=("Times New Roman", 12))
        label_agradecimento.place(relx=0.15, rely=0.85, relheight=0.10, relwidth=0.73)

    def frames(self):
        self.frame_centro = Frame(self, bg = self.cor_tela)
        self.frame_centro.place(relx=0.10, rely=0.25, relheight=0.55, relwidth=0.8) 

        label_nomeLoja=Label(self, text="NOME DA LOJA: LOJA DE GÁS", fg = self.cor_fonte, bg = self.cor_botao, font=("Times New Roman", 9)) #bg = cor da tela, fg = cor da fonte 
        label_nomeLoja.place(relx=0.13, rely=0.27, relheight=0.12, relwidth=0.73)           

        label_numeroTelefone=Label(self, text="NÚMERO DE TELEFONE: \n 3353-7890 / (24) 99866-8904", fg = self.cor_fonte, bg = self.cor_botao, font=("Times New Roman", 9))
        label_numeroTelefone.place(relx=0.13, rely=0.34, relheight=0.10, relwidth=0.73) 

        label_cidade=Label(self, text="CIDADE: RESENDE", fg = self.cor_fonte, bg = self.cor_botao, font=("Times New Roman", 9))
        label_cidade.place(relx=0.13, rely=0.41, relheight=0.12, relwidth=0.73)

        label_endereco=Label(self, text="ENDEREÇO: PARAÍSO - RUA DAS PALMEIRAS", fg = self.cor_fonte, bg = self.cor_botao, font=("Times New Roman", 9))
        label_endereco.place(relx=0.13, rely=0.48, relheight=0.14, relwidth=0.73)

        label_preco=Label(self, text="PREÇO DO GÁS: R$ 75,00", fg = self.cor_fonte, bg = self.cor_botao, font=("Times New Roman", 9))
        label_preco.place(relx=0.13, rely=0.56, relheight=0.14, relwidth=0.73)

        label_promocoes=Label(self, text="PROMOÇÕES: CASO TENHA UMA", fg = self.cor_fonte, bg = self.cor_botao, font=("Times New Roman", 9))
        label_promocoes.place(relx=0.13, rely=0.64, relheight=0.14, relwidth=0.73)   

    def fechar(self):
        self.destroy()
        print('APERTOU FECHAR')         

class Confirmar(Toplevel): 
    cor_tela = '#3F7958' # verde
    cor_root = '#656D4A' # verde 
    cor_2 = '#E2E237' # amarelo 
    cor_fonte = '#000000' # preto 
    cor_botao = '#FFFFFF' # branco 

    def __init__(self, original):
        self.frame_original = original 
        Toplevel.__init__(self)
        self.geometry('375x600+975+10')
        self.configure(bg = self.cor_botao)
        self.title("MCM GÁS")
        self.widgets()
        self.frames()  

    def widgets(self):
        label_mcm=Label(self, text="MCM GÁS", bg=self.cor_botao, font=("Broadway", 22))  
        label_mcm.place(relx=0, rely=0, relheight=0.20, relwidth=1.0)

    def frames(self):
        self.frame_centro = Frame(self, bg = self.cor_tela)
        self.frame_centro.place(relx=0.10, rely=0.25, relheight=0.55, relwidth=0.8) 

        label_nomeLoja=Label(self, text="NOME DA LOJA: LOJA DE GÁS", fg = self.cor_fonte, bg = self.cor_botao, font=("Times New Roman", 9)) #bg = cor da tela, fg = cor da fonte 
        label_nomeLoja.place(relx=0.13, rely=0.27, relheight=0.12, relwidth=0.73)           

        label_numeroTelefone=Label(self, text="NÚMERO DE TELEFONE: \n 3353-7890 / (24) 99866-8904", fg = self.cor_fonte, bg = self.cor_botao, font=("Times New Roman", 9))
        label_numeroTelefone.place(relx=0.13, rely=0.34, relheight=0.10, relwidth=0.73) 

        label_cidade=Label(self, text="CIDADE: RESENDE", fg = self.cor_fonte, bg = self.cor_botao, font=("Times New Roman", 9))
        label_cidade.place(relx=0.13, rely=0.41, relheight=0.12, relwidth=0.73)

        label_endereco=Label(self, text="ENDEREÇO: PARAÍSO - RUA DAS PALMEIRAS", fg = self.cor_fonte, bg = self.cor_botao, font=("Times New Roman", 9))
        label_endereco.place(relx=0.13, rely=0.48, relheight=0.14, relwidth=0.73)

        label_preco=Label(self, text="PREÇO DO GÁS: R$ 75,00", fg = self.cor_fonte, bg = self.cor_botao, font=("Times New Roman", 9))
        label_preco.place(relx=0.13, rely=0.56, relheight=0.14, relwidth=0.73)

        label_promocoes=Label(self, text="PROMOÇÕES: CASO TENHA UMA", fg = self.cor_fonte, bg = self.cor_botao, font=("Times New Roman", 9))
        label_promocoes.place(relx=0.13, rely=0.64, relheight=0.14, relwidth=0.73)

        self.btn_voltar = Button(self, text="CONFIRMAR PEDIDO", font=("Times New Roman", 13), fg=self.cor_tela, bg=self.cor_2, command=self.agradecimento)
        self.btn_voltar.place(relx = 0.28, rely = 0.90)

    def agradecimento(self): 
        self.hide() # esconder a tela atual 
        self.subFrame = Agradecimento(self)

    def hide(self): # Esconde o root (tela principal)
        self.withdraw() 

    def show(self): # Mostra outra janela 
        self.update() 
        self.deiconify()  

class Pedidos(Toplevel):
    cor_tela = '#3F7958' # verde
    cor_root = '#656D4A' # verde 
    cor_2 = '#E2E237' # amarelo 
    cor_fonte = '#000000' # preto 
    cor_botao = '#FFFFFF' # branco 
    cor_laranja = '#F48C06' #laranja                 

    def __init__(self, original):
        self.frame_original = original 
        Toplevel.__init__(self)
        self.geometry('375x600+975+10')  
        self.configure(bg = self.cor_tela) 
        self.title("         MCM GÁS        ") 
        self.widgets()
          

    def widgets(self):
        label_lojaA=Label(self, text="MCM GÁS", bg = self.cor_2, font=("Broadway", 22))  
        label_lojaA.place(relx=0, rely=0, relheight=0.10, relwidth=1.0)

        label_lojaA=Label(self, text="LOJA A", fg = self.cor_2, bg = self.cor_tela, font=("Times New Roman", 12, BOLD))
        label_lojaA.place(relx=0, rely=0.12, relheight=0.1, relwidth=0.99)  

        self.img_gas=PhotoImage(file="gas.png")
        label_imagem=Label(self, image=self.img_gas)
        label_imagem.place(relx=0.10, rely=0.20, relheight=0.27, relwidth=0.8) 

        label_preco=Label(self, text="PREÇO: R$75,00", bg = self.cor_tela, font=("Times New Roman", 11))
        label_preco.place(relx=0, rely=0.40, relheight=0.1, relwidth=0.99)

        label_pagamento=Label(self, text="FORMA DE PAGAMENTO: \n Dinheiro, débito", bg = self.cor_tela, font=("Times New Roman", 11))
        label_pagamento.place(relx=0, rely=0.50, relheight=0.1, relwidth=0.99)

        label_endereco=Label(self, text="ENDEREÇO: \n Rua das Palmeiras - Paraíso", bg = self.cor_tela, font=("Times New Roman", 11))
        label_endereco.place(relx=0, rely=0.60, relheight=0.1, relwidth=0.99)

        label_telefone=Label(self, text="TELEFONE PARA CONTATO: \n (00) 000000-0000", bg = self.cor_tela, font=("Times New Roman", 11))
        label_telefone.place(relx=0, rely=0.70, relheight=0.1, relwidth=0.99)

        label_descricao=Label(self, text="DESCRIÇÃO: ", bg = self.cor_tela, font=("Times New Roman", 11))
        label_descricao.place(relx=0, rely=0.80, relheight=0.1, relwidth=0.99)

        self.btn_voltar = Button(self, text="FAZER PEDIDO", font=("Times New Roman", 13), bg=self.cor_laranja, command=self.confirmar)
        self.btn_voltar.place(relx = 0.30, rely = 0.90)

    def confirmar(self):
        self.hide() # esconder a tela atual 
        self.subFrame = Confirmar(self) 

    def hide(self): # Esconde o root (tela principal)
        self.withdraw() 

    def show(self): # Mostra outra janela 
        self.update() 
        self.deiconify()   

class TelaOfertas(Toplevel):
    cor_tela = '#3F7958' # verde
    cor_root = '#656D4A' # verde 
    cor_2 = '#E2E237' # amarelo 
    cor_fonte = '#000000' # preto 
    cor_botao = '#FFFFFF' # branco 

    def __init__(self, original): 
        self.frame_original = original 
        Toplevel.__init__(self) #importando método construtor   
        self.geometry('375x600+975+10')  
        self.configure(bg = self.cor_botao) #largura(375) x altura(600) + posição horizontal + pos ver 
        self.title("         MCM GÁS        ") 
        self.widgets()
        self.frames()
        self.widgetsframe_menuinferior()

    def widgets(self): 
        label_aviso=Label(self, text="Lojas não cadastradas não estão habilitadas para \n fazer pedidos, apenas visualização.", bg = self.cor_botao, font=("Times New Roman", 11))
        label_aviso.place(relx=0.03, rely=0.05, relheight=0.05, relwidth=0.95)

        label_lojaa=Label(self, text="Loja cadastrada  \n LOJA A - R$ 75,00", bg = self.cor_tela, font=("Times New Roman", 12))
        label_lojaa.place(relx=0.10, rely=0.15, relheight=0.1, relwidth=0.80) 

        label_lojab=Label(self, text="Loja não cadastrada  \n LOJA B - R$ 78,99", bg = self.cor_2, font=("Times New Roman", 12))
        label_lojab.place(relx=0.10, rely=0.28, relheight=0.1, relwidth=0.80)

        label_lojab=Label(self, text="Loja cadastrada  \n LOJA C - R$ 97,00", bg = self.cor_tela, font=("Times New Roman", 12))
        label_lojab.place(relx=0.10, rely=0.41, relheight=0.1, relwidth=0.80)

        label_lojab=Label(self, text="Loja cadastrada  \n LOJA D - R$ 109,00", bg = self.cor_tela, font=("Times New Roman", 12))
        label_lojab.place(relx=0.10, rely=0.54, relheight=0.1, relwidth=0.80)

        label_lojab=Label(self, text="Loja cadastrada  \n LOJA E - R$ 80,00", bg = self.cor_tela, font=("Times New Roman", 12))
        label_lojab.place(relx=0.10, rely=0.67, relheight=0.1, relwidth=0.80)
        
        self.btn_voltar = Button(self, text="Registrar compra do usuário", font=("Times New Roman", 13), bg=self.cor_2, command=self.onClose)
        self.btn_voltar.place(relx = 0.25, rely = 0.84)

    def frames(self): 
        self.frame_menuinferior=Frame(self, bg = self.cor_tela)
        self.frame_menuinferior.place(relx=0, rely=0.9, relheight=0.10, relwidth=100)

    def widgetsframe_menuinferior(self):
        self.label_icone = Label(self.frame_menuinferior, text="ícone", font=("Times New Roman", 12))
        self.label_icone.place(relx=0.10, rely=0.05, relheight=0.10, relwidth=1.0 )

        label_icone_casa = Label(self.frame_menuinferior, text='Oi', bg='blue')
        label_icone_casa.pack()


    def onClose(self): 
        self.destroy() #sai da memória, diferente do hide que apenas "esconde" da memória 
        self.subFrame = Pedidos(self)    
 
class App:
    # CORES DO APP
    cor_tela = '#3F7958' # verde
    cor_root = '#656D4A' # verde 
    cor_2 = '#E2E237' # amarelo 
    cor_fonte = '#000000' # preto 
    cor_botao = '#FFFFFF' # branco 

    def __init__(self): # o que vai rodar 
        self.root = root 
        self.tela()
        self.widgets()
        
        root.mainloop() 

    def tela(self): # método config. da tela 
        self.root.geometry('375x600+975+10')
        self.root.configure(bg = self.cor_tela) # largura(375) x altura(600) + posição horizontal + pos ver 
        self.root.title("         MCM GÁS        ")

    def widgets(self): 
        # texto
        # entrada de texto 
        # botão

        self.cadastro=Label(self.root, text="Cadastro", font=("Times New Roman", 20), bg=self.cor_tela)
        self.cadastro.place(relx=0.35, rely=0.07) 

        self.mcmgas=Label(self.root, text="MCM GÁS", font=("Broadway", 18), bg=self.cor_2)
        self.mcmgas.place(relx=0, rely=0, relheight=0.06, relwidth=1.0)    
         
        self.texto=Entry(self.root, font=("Times New Roman", 13))
        self.texto.place(relx=0.28, rely=0.13)

        self.nome_entry=Entry(self.root, font=("Times New Roman", 13))
        self.nome_entry.place(relx=0.28, rely=0.23)

        label_nome=Label(self.root, text="Nome:", bg=self.cor_tela)
        label_nome.place(relx=0.15, rely=0.13)

        self.email_entry=Entry(self.root, font=("Times New Roman", 13), show="*")
        self.email_entry.place(relx=0.28, rely=0.33)

        label_email=Label(self.root, text="E-mail:", bg=self.cor_tela)
        label_email.place(relx=0.15, rely=0.23)

        self.senha=StringVar()
        self.senha_entry=Entry(self.root, textvariable=self.senha, show="*")
        self.senha_entry.place(relx=0.28, rely=0.43, relheight=0.04, relwidth=0.49)

        label_senha=Label(self.root, text="Senha:", bg=self.cor_tela)
        label_senha.place(relx=0.15, rely=0.33)

        self.confirme_sua_senha_entry=Entry(self.root, font=("Times New Roman", 13))
        self.confirme_sua_senha_entry.place(relx=0.28, rely=0.53)

        label_confirmar=Label(self.root, text="Confirmar:", bg=self.cor_tela) 
        label_confirmar.place(relx=0.10, rely=0.43)

        self.cep_entry=Entry(self.root, font=("Times New Roman",13))
        self.cep_entry.place(relx=0.28, rely=0.63)

        label_cep=Label(self.root, text="CEP:", bg=self.cor_tela)
        label_cep.place(relx=0.15, rely=0.53)

        self.endereco_entry=Entry(self.root, font=("Times New Roman",13))
        self.endereco_entry.place(relx=0.28, rely=0.73)

        label_endereco=Label(self.root, text="End.:", bg=self.cor_tela)
        label_endereco.place(relx=0.15, rely=0.63)

        self.cpf_entry=Entry(self.root, font=("Times New Roman",13))
        # self.cpf_entry.place(relx=0.28, rely=0.83)

        label_cpf=Label(self.root, text="CPF:", bg=self.cor_tela)
        label_cpf.place(relx=0.15, rely=0.73)

        self.btn_cadastrar = Button(self.root, text = "CADASTRAR", font=("Times New Roman",13), command = self.entrar_tela_ofertas)
        self.btn_cadastrar.place(relx = 0.35, rely = 0.90)

    

    def entrar_tela_ofertas(self):
        self.hide() # esconder a tela atual 
        self.subFrame = TelaOfertas(self) 

    def hide(self): # Esconde o root (tela principal)
        self.root.withdraw() 

    def show(self): # Mostra outra janela 
        self.root.update() 
        self.root.deiconify()         

    def fechar(self):
        self.root.destroy()
        print('APERTOU FECHAR')

### programa principal ### 
root = Tk() 
App()                                   


Protótipo do Aplicativo MCM Gás! 
