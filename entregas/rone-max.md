# Laudo Técnico de Armazenamento – Hiren's BootCD PE v1.0.8

* **Técnico Responsável:** Rone Max 
* **Data da Execução:** 26/11/2026
* **VM Utilizada:** `HBCD-v1.0.8`

---

## 1. Particionamento e Formatação (AOMEI / DiskGenius)

| Parâmetro Configurado | Valor Aplicado |
| :--- | :--- |
| **Disco Alvo** | Disk 1 (20 GB VDI) |
| **Tabela de Partição** | GPT |
| **Sistema de Arquivos** | NTFS |
| **Letra Atribuída** | `D:\` |

**Evidência 1 – Gerenciador de Partições:**
![Particionamento GPT NTFS](img/seu-nome-particao.png)

---

## 2. Análise de Saúde S.M.A.R.T. (CrystalDiskInfo)

* **O CrystalDiskInfo exibiu os atributos S.M.A.R.T. do disco de 20 GB?** Não
* **Justificativa Técnica: CrystalDiskInfo não reconheceu o disco virtual do virtualbox (mensagem Disk Not found

## 3. Teste de Desempenho de Leitura (HD Tune Benchmark)

| Métrica Aferida | Resultado Obtido |
| :--- | :--- |
| **Taxa Mínima (Minimum)** 110.5 MB/s |
| **Taxa Máxima (Maximum)** 134.0 MB/s |
| **Taxa Média (Average)** 129.1 MB/s |
| **Tempo de Acesso (Access Time)** 0.5ms |

**Evidência 2 – Gráfico do Benchmark:**
![Benchmark HD Tune](img/seu-nome-benchmark.png)
