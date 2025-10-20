# 🧩 Mini-Projeto — Diagnóstico e Correção de Conectividade IPv4

## 🎯 Objetivo
Avaliar a capacidade do aluno em diagnosticar e corrigir problemas de conectividade IPv4 **utilizando exclusivamente o PowerShell**, sem recorrer a interfaces gráficas.

---

## 🧠 Cenário
A rede da filial de **Londres** apresenta dois problemas de comunicação:

| Computador | Sintoma | Observação |
|-------------|----------|-------------|
| **LON-CL1** | Não comunica com nenhum outro host | O IP atribuído é APIPA (169.254.x.x). |
| **LON-CL2** | Consegue aceder ao servidor local (LON-DC1), mas não à sede (TOR-SVR1) | O gateway está incorreto. |

O aluno deve diagnosticar, corrigir e validar a conectividade IPv4 entre os hosts.

---

## 🧩 Tarefas a Realizar (via PowerShell)

### 🔹 Parte 1 – Diagnóstico
1. Testar conectividade com `LON-DC1` e `TOR-SVR1`:
   ```powershell
   Test-NetConnection LON-DC1
   Test-NetConnection TOR-SVR1
