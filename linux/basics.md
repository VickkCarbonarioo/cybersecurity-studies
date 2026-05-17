# Linux Basics

## Comandos aprendidos

### pwd
Mostra em qual diretório/pasta você está.

### ls
Lista arquivos e pastas.

### ls -la
Lista arquivos mostrando:
- permissões
- arquivos ocultos
- dono
- detalhes

### mkdir
Cria uma pasta.

Exemplo:
```bash
mkdir estudos-cyber
```

### cd
Entra em uma pasta.

Exemplo:
```bash
cd estudos-cyber
```

### cd ..
Volta uma pasta/diretório.

### touch
Cria um arquivo vazio.

Exemplo:
```bash
touch anotacoes.txt
```

### nano
Editor de texto dentro do terminal.

Exemplo:
```bash
nano anotacoes.txt
```

Atalhos:
- CTRL + O → salvar
- CTRL + X → sair

### cat
Mostra o conteúdo de um arquivo.

Exemplo:
```bash
cat anotacoes.txt
```

---

# Redes e Cybersecurity

## O que é IP
É como o endereço de uma casa na rede.

## O que é porta
É como um cômodo/porta específica da casa.

## Interfaces de rede

### lo
Loopback / localhost.
O computador falando consigo mesmo.

IP:
```text
127.0.0.1
```

### eth0
Interface de rede da máquina virtual.

---

# Nmap

Ferramenta utilizada para:
- descobrir portas abertas
- reconhecimento de rede
- identificar serviços
- mapear dispositivos

## Fast Scan

```bash
nmap -F scanme.nmap.org
```

O parâmetro `-F` faz um scan mais rápido.
