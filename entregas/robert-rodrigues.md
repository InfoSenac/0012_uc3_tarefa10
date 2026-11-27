# Laudo Técnico de Armazenamento – Hiren's BootCD PE v1.0.8

* **Técnico Responsável:** `Robert Rodrigues Rosa Magalhães`
* **Data da Execução:** `25/11/2026`
* **VM Utilizada:** `HBCD-v1.0.8`

---

## 1. Particionamento e Formatação (AOMEI / DiskGenius)

| Parâmetro Configurado | Valor Aplicado |
| :--- | :--- |
| **Disco Alvo** | Disk 1 (20 GB VDI) |
| **Tabela de Partição** | GPT |
| **Sistema de Arquivos** | NTFS |
| **Letra Atribuída** | `C:\` |

**Evidência 1 – Gerenciador de Partições:**
![Particionamento GPT NTFS](img/robert-particao.png)

---

## 2. Análise de Saúde S.M.A.R.T. (CrystalDiskInfo)

* **O CrystalDiskInfo exibiu os atributos S.M.A.R.T. do disco de 20 GB?** Não
* **Justificativa Técnica:** o S.M.A.R.T. pertence ao hardware físico. O disco virtual representa o armazenamento, mas não necessariamente transmite os sensores e diagnósticos do dispositivo real.

---

## 3. Teste de Desempenho de Leitura (HD Tune Benchmark)

| Métrica Aferida | Resultado Obtido |
| :--- | :--- |
| **Taxa Mínima (Minimum)** | 25.3 MB/s |
| **Taxa Máxima (Maximum)** | 123.6 MB/s |
| **Taxa Média (Average)** | 118.2 MB/s |
| **Tempo de Acesso (Access Time)** | 0.6 ms |

**Evidência 2 – Gráfico do Benchmark:**
![Benchmark HD Tune](img/robert-benchmark.png)