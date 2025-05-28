## Desafio Prático – Desenvolvedor Brew

### **Descrição do Desafio**

Você deve desenvolver uma aplicação web simples com **Laravel**, **Blade e/ou Livewire** e **Tailwind CSS** com as seguintes funcionalidades:

---

## Funcionalidades obrigatórias

### **Autenticação**

* Implementar um **sistema de login**.
* Apenas **usuários autenticados** podem acessar as telas de produtos.

---

### **CRUD de Produtos**

Cada produto deve conter os seguintes campos:

* **Nome** (string)
* **SKU** (string)
* **Imagem** (upload ou URL)
* **Ativo** (boolean)
* **Preço** (decimal)
* **Estoque** (inteiro)
* **Criado por** (nome do usuário que criou)
* **Data de criação** (timestamp)
* **Data de atualização** (timestamp)

---

### **Funcionalidades específicas do CRUD**

* **Listagem** de produtos com:

  * Campo de **busca** por `Nome` ou `SKU`.
  * **Ordenação** por qualquer coluna.
  * Indicação de status (Ativo/Inativo).

* **Criação** de produtos:

  * Formulário simples.
  * Exibir **mensagem de feedback** de sucesso ou erro.

* **Edição** de produtos:

  * Feita através de um **modal**.
  * Mensagem de feedback após a atualização.

* **Deleção** de produtos:

  * Deve solicitar uma **confirmação** antes de excluir.

---

## Stacks obrigatórias

* **Laravel** (versão livre, sugerimos a mais recente).
* **Tailwind CSS** para toda a estilização.
* **Blade** e/ou **Livewire** para componentização.

---

## Considerações extras

* **Componentização** será avaliada: use componentes de Blade ou Livewire sempre que possível.
* A aplicação deve ser **responsiva**.
* A listagem deve ter **paginação** (não precisa ser infinita, pode ser padrão do Laravel).

---

## Será considerado um diferencial:

* Implementar **testes automatizados** básicos com **PEST PHP**.
* Utilizar **Livewire** para interatividade (principalmente na busca, ordenação e modal).
* UX bem resolvida: modais fluidos, mensagens de feedback claras.
* Utilização de validação dos campos dos formulários.
* Uso de **Soft Deletes** para a deleção de produtos.

---

## Entrega

* Disponibilizar o código em um **repositório público no GitHub**.
* Incluir um **README** explicando:

  * Como rodar o projeto.
  * Tecnologias utilizadas.
  * Quais funcionalidades obrigatórias e opcionais foram implementadas.

---

## Critérios de Avaliação

* Estrutura e organização do código.
* Fidelidade aos requisitos.
* Clareza na implementação.
* Uso adequado de **Laravel** e **Tailwind**.
* Atenção à UX e responsividade.
* Implementação de diferenciais.

---

## Exemplo de fluxo esperado:

1. Usuário acessa `/login`, se autentica.
2. Redireciona para `/produtos`.
3. Vê a lista de produtos com busca, ordenação e paginação.
4. Clica em **Editar** → modal abre → edita → vê mensagem de sucesso.
5. Clica em **Excluir** → confirmação → produto excluído.
6. Clica em **Novo Produto** → formulário → cria → vê mensagem de sucesso.

---

## Restrições

* Não usar pacotes prontos de CRUD.
* Não usar Admin Panels automáticos como Laravel Nova, Filament, etc.
* O foco é demonstrar domínio da stack e boas práticas.

