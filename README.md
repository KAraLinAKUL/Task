# Task
My repo for lesson
import random
def lista_2D(liczba1, liczba2):
    lista_dwumywiarowa = []
    for i in range(3):
        wiersz = []
        for j in range(7):
            wiersz.append(random.randint(0,100))
        lista_dwumywiarowa.append(wiersz)
    return lista_dwumywiarowa
def najwiekszy(lista):
    najwiekszy = lista[0][0]
    for wiersz in lista:
        for element in wiersz:
            if element > najwiekszy:
                najwiekszy = element
    return najwiekszy
moja_lista = lista_2D(3, 4)
print(moja_lista)
najwiekszy_element = najwiekszy(moja_lista)
print(najwiekszy_element)
