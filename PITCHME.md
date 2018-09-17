# Flux

An application architecture for React

---

@snap[west span-60]

@ul[](false)
- Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
- Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi
- Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
- Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
@ulend

@snapend

@snap[east span-30]
something
@snapend
---

@snap[west text-orange span-50]
Topics to be covered today
@snapend

@snap[east text-white span-45]

@ol
- Lorem ipsum dolor sit amet, consectetur elit
- Ut enim ad minim veniam, quis exercitation
- Duis aute irure dolor in reprehenderit in voluptate
@olend

@snapend

---

@snap[north text-white span-100]
@size[1.5em](Por que seguir boas práticas?)
@snapend

@snap[south span-100]
@ul[](false)
- software nunca está pronto. Depois de entregue, precisa de manutenção
- todo software tem bugs :/
- código é lido muito mais vezes do que alterado: legibilidade é importante
- você não sabe quem irá alterar esse código no futuro, qual o contexto da pessoa. Pode ser você mesmo, sem lembrar do contexto em que está agora
@ulend
@snapend

---

### Flux Design

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

+++

![Flux Explained](https://facebook.github.io/flux/img/flux-simple-f8-diagram-explained-1300w.png)

---

## Nomes

Nomes devem revelar uma intenção

<pre><code class="lang-python hljs">
def get_them():
  list1 = []
  for x in the_list:
    if x[0] == 4:
      list1.append(x)
  return list1
</code></pre>

<pre class="fragment" data-fragment-index="1"><code class="lang-python hljs">
def get_flagged_cells():
  flagged_cells = []
  for cell in game_board:
    if cell[STATUS_VALUE] == FLAGGED:
      flagged_cells.append(cell)
  return flagged_cells
</code></pre>
