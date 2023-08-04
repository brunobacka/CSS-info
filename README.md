# Combinador direto
Repositório criado para listar algumas resolução de dúvidas de CSS
```
# Combinador Direto

maior que '>' - seleciona apenas os filhos diretos daquele seletor, ex:


---html---

<div class="pai"> pai
  <div class"filho"> filho
    <div class="filho"> filho do filho (neto)</div>
  </div>
</div>

---CSS---

.pai .filho {
  color:orange;
]


#Combinador descendente normal#
Dessa forma ambos abaixo do pai receberão o atributo de cor do CSS

pai
>filho
>>neto


---html---

<div class="pai"> pai
  <div class"filho"> filho
    <div class="filho"> filho do filho (neto)</div>
  </div>
</div>

---CSS---

.pai > .filho {
  color:orange;
]

#Combinador descendente direto#
Dessa forma apenas os filho direto vai receber o atributo de cor do CSS

pai
>filho - recebe o atributo
neto


---html---

<div class="pai"> pai
  <div class"filho"> filho
    <div class="filho"> filho do filho (neto)</div>
  </div>
</div>

---CSS---

.pai > .filho > .filho{
  color:orange;
]

#combinador descendente do pai#
Dessa forma o neto vai receber o atributo de cor do CSS

pai
filho
>Neto - recebe atributo
