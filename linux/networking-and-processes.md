# Networking and Processes

# Python HTTP Server

## Criando um servidor simples

```bash
python3 -m http.server 8080
```

Cria um servidor web simples usando Python na porta 8080.

A máquina fica "escutando" conexões nessa porta.

Acessando:
```text
http://localhost:8080
```

é possível visualizar os arquivos da pasta no navegador.

---

# Nmap

## Escaneando uma porta específica

```bash
nmap -p 8080 localhost
```

### Explicação

- `-p`
  - especifica qual porta será escaneada

- `localhost`
  - a própria máquina
  - IP:
```text
127.0.0.1
```

Quando o servidor Python estava ativo, o Nmap mostrou:

```text
8080/tcp open
```

Indicando que existia um serviço rodando e escutando naquela porta.

---

# lsof

## Verificando qual processo está usando uma porta

```bash
sudo lsof -i :8080
```

### Explicação

- `sudo`
  - executa como administrador/root

- `lsof`
  - List Open Files

- `-i`
  - relacionado à rede/internet

- `:8080`
  - filtra pela porta 8080

Esse comando mostra qual processo está utilizando determinada porta.

---

# ps aux

## Listando processos do sistema

```bash
ps aux
```

Semelhante ao Gerenciador de Tarefas do Windows.

### Explicação

- `ps`
  - process status

- `a`
  - mostra processos de todos os usuários

- `u`
  - mostra detalhes e dono dos processos

- `x`
  - mostra processos sem terminal também

---

# grep

## Filtrando resultados

```bash
ps aux | grep python
```

### Pipe `|`

O pipe pega a saída do primeiro comando e envia para o próximo comando.

### grep

O `grep` procura palavras específicas.

No exemplo acima:
- `ps aux`
  - lista todos os processos

- `|`
  - envia o resultado para o próximo comando

- `grep python`
  - filtra apenas linhas contendo "python"

Isso permite localizar processos específicos no sistema.
