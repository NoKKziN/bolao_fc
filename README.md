# ⚽ BolãoFC

O **BolãoFC** é um site de **bolão de futebol** totalmente integrado ao **Supabase**, desenvolvido para permitir o cadastro de usuários, partidas e palpites, além de acompanhar a classificação dos participantes.  
O projeto demonstra um **CRUD completo** e o uso prático de banco de dados em uma aplicação web moderna e responsiva.

🔗 **Acesse o site:** [https://bolao-fut-scores.lovable.app/](https://bolao-fut-scores.lovable.app/)

---

## 🧭 Funcionalidades Principais

- **Página de Partidas:**  
  Lista todas as partidas cadastradas, exibindo informações como local, data, hora e placar final (quando disponível).  
  Permite que o usuário insira palpites e visualize palpites de outros participantes.

- **Página de Palpites:**  
  Exibe todos os palpites feitos, mostrando o nome do usuário, a partida e os resultados apostados.  
  Permite **criar, editar e excluir palpites** (CRUD completo).

- **Página de Classificação:**  
  Mostra o ranking dos usuários com base em uma **view ou função RPC** chamada `classificacao`, que retorna os campos `usuario` e `pontos`.

- **Página de Administração:**  
  Área de gerenciamento completa para adicionar, editar e remover:
  - Usuários  
  - Partidas (com data e hora)  
  - Palpites

- **Modo Claro e Escuro:**  
  O site conta com um botão que alterna entre os modos visual e escuro, proporcionando melhor experiência de uso.

---

## 💾 Integração com Supabase

O sistema está conectado ao banco de dados **Supabase**, utilizando as seguintes tabelas:

- `usuarios(id_usuario, nome, email)`  
- `partidas(id_partida, created_at, local, time_casa, time_fora, data_partida, hora_partida, placar_casa, placar_fora)`  
- `palpites(id, usuario_id, partida_id, placar_casa, placar_fora)`

E uma função ou view para classificação:
- `classificacao(usuario, pontos)`

Todas as operações de **CRUD (Create, Read, Update, Delete)** são realizadas diretamente via Supabase Client.

---

## 🧱 Tecnologias Utilizadas

- **Frontend:** React (Lovable)  
- **Banco de Dados:** Supabase (PostgreSQL)  
- **Estilização:** Tailwind CSS  
- **Animações:** Framer Motion  
- **Ícones:** Lucide Icons  

---

## 🎨 Design e Navegação

- Layout **limpo, moderno e responsivo**
- **Cores neutras** e **botões azuis** (`#1E88E5`)
- Barra de navegação superior com os links:
  - **Partidas**
  - **Palpites**
  - **Classificação**
- Título principal: **BolãoFC**
- Componentes com cantos arredondados, sombras suaves e espaçamento adequado

---

## 🖼️ Prints e Modelo Lógico

### 🧩 Modelo Lógico do Banco de Dados
<img width="873" height="666" alt="image" src="https://github.com/user-attachments/assets/4ceeb9ca-2059-46b5-9f77-9bf3fdfd8e0a" />


---

### 🏠 Tela Principal
<img width="1899" height="847" alt="image" src="https://github.com/user-attachments/assets/54bfe50d-6e15-40ae-b98f-d972938dd39c" />

<img width="1902" height="913" alt="image" src="https://github.com/user-attachments/assets/bad638ba-7190-4a2b-9d96-a23db171f0c4" />


---

### ⚽ Tela de Partidas
<img width="1919" height="915" alt="image" src="https://github.com/user-attachments/assets/f9eb4416-a9b1-4dc3-8ba9-812ca0b4d765" />

<img width="1919" height="912" alt="image" src="https://github.com/user-attachments/assets/237a7827-11bf-43dc-975a-5fd9673435a3" />


---

### 🧾 Tela de Palpites
<img width="1917" height="916" alt="image" src="https://github.com/user-attachments/assets/ef9e354c-bd07-4b7b-905e-141221638395" />

<img width="1919" height="911" alt="image" src="https://github.com/user-attachments/assets/7f4123d5-6891-4197-832d-6c15b28341db" />


---

### 🏆 Tela de Classificação
<img width="1919" height="910" alt="image" src="https://github.com/user-attachments/assets/1ddeb90d-00db-4ea5-a501-2d958f440168" />

<img width="1919" height="915" alt="image" src="https://github.com/user-attachments/assets/8f3c43cc-64fa-4215-887c-fa72cf8ba438" />


---

### 🛠️ Tela de Administração
<img width="1919" height="913" alt="image" src="https://github.com/user-attachments/assets/52b439b3-32dc-44a4-8cdb-0f163a7236fc" />

<img width="1919" height="913" alt="image" src="https://github.com/user-attachments/assets/41cb3e53-9e04-41ed-898f-2c00d557e7ae" />

