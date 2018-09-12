# Flux

An application architecture for React

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

<div class="left">
```python
def get_them():
  list1 = []
  for x in the_list:
    if x[0] == 4:
      list1.append(x)
  return list1
```
</div>

<div class="right">
```python
def get_flagged_cells():
  flagged_cells = []
  for cell in game_board:
    if cell[STATUS_VALUE] == FLAGGED:
      flagged_cells.append(cell)
  return flagged_cells
```
</div>
