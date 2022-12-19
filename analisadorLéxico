import re

tokens = ['if',
'elif', 
'else', 
'for',
'while', 
'True', 
'False', 
'print', 
'input', 
'break', 
'continue']

delimitador = [',', '{', '}', ';', ':']

expressão = input("Digite a expressão: ")


def separaString(i):
    separa = re.split(r'\s', i)
    if separa is None:
        return None
    if separa:
        return separa

def numeroPositivo(i):
    positivo = re.compile(r'\d*')
    busca = re.search(positivo, i)
    if busca:
        return True
    else:
        return False

def numeroNegativo(i):
    negativo = re.compile(r'^-\d*\d$')
    busca = re.search(negativo, i)
    if busca:
        return True
    else:
        return False

def letra(i):
    letras = re.compile(r'[a-zA-Z]')
    busca = re.search(letras, i)
    if busca:
        return True
    else:
        return False

if expressão not in tokens:
    separada = separaString(expressão)
    print(" EXPRESSÃO COMPLETA: \n"+str(separada))

    for i in separada:
        if numeroNegativo(i):
            print("("+str(i)+") NÚMERO (NEGATIVO)")
        elif i == '+':
            print("(+) -> OPERADOR DE SOMA")
        elif i == '-':
            print("(-) -> OPERADOR DE SUBTRAÇÃO")
        elif i == '*':
            print("(*) -> OPERADOR DE MULTIPLICAÇÃO")
        elif i == '**':
            print("(**) -> OPERADOR DE EXPONENCIAÇÃO")
        elif i == '/':
            print("(/) -> OPERADOR DE DIVISÃO")
        elif i == ')':
            print(" ) -> DELIMITADOR PARENTESES")
        elif i == '(':
            print(" ( -> DELIMITADOR PARENTESES")
        elif i in delimitador:
            print(f"{i} -> DELIMITADOR")
        elif letra(i):
            print("("+i+") -> STRING")
        elif numeroPositivo(i):
            print("("+str(i)+") -> NUMERO (POSITIVO)")
        else:
            print('Caractere Invalido')

elif expressão in tokens:
    print('PALAVRA RESERVADA: ')
    if expressão == 'if':
        print('if : pega_visao')
    elif expressão == 'elif':
        print('elif : migué')
    elif expressão == 'else':
        print('else : se_pique')
    elif expressão == 'for':
        print('for : barril')
    elif expressão == 'while':
        print('while : barril_dobrado')
    elif expressão == 'break':
        print('break : acabou_a_brincadeira')
    elif expressão == 'continue':
        print('continue : segue')
    elif expressão == 'True':
        print('True : ésim')
    elif expressão == 'False':
        print('False : laranjada')
    elif expressão == 'print':
        print('print = mostrae')
    elif expressão == 'input':
        print('input = colocae')
