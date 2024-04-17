# Estimativa de custo de implantação dos 3 serviços AWS

Data: 17/04/2024

Empresa: Abstergo Industries

Responsável: Victor Sérgio Silva Barros

## Introdução
Foi utilizada a **Calculadora de Preços da AWS**. Essa ferramenta permite explorar os serviços da AWS e criar uma estimativa dos custos para os seus casos de uso específicos.
## Descrição dos serviços

1. AWS EC2 Auto Scaling**:
   - O **Auto Scaling** permite ajustar automaticamente o número de instâncias EC2 com base na demanda.
   - O custo está relacionado ao uso das instâncias EC2 e às configurações de escalabilidade.
   - O **Amazon EC2** é um serviço de computação em nuvem que permite criar e gerenciar instâncias de máquinas virtuais.
   - O custo do EC2 varia com base no tipo de instância (por exemplo, t2.micro, m5.large), região, sistema operacional e opções de armazenamento.

	Descrição do serviço:<br>
	Região: américa do Sul (São Paulo)
	Locação:Instâncias compartilhadas
	Sistema operacional: Linux
	Cargas de trabalho: Pico de tráfego diário
	Baseline: 1
	Peak: 2
	Duração do pico (horas, minutos): Hours: 8 - Minutes:30

	Instância escolhida: t4g.nano | Family: t4g | 2vCPU | 0.5 GiB Memória

	Custo inicial total: 0.00 USD <br>
	Custo mensal total: **3.89 USD**
	
	
2. **Amazon RDS**:
   - O **Amazon RDS** é um serviço de banco de dados relacional gerenciado.
   
   Descrição do serviço:<br>
   Especificações da instâncias MariaDB<br>
	
	Instância escolhida: db.m3.2xlarge
	vCPU: 8 | 
	Memory: 30 GiB | 
	1 instância(s) x 1.88 USD por hora x (12 / 24 horas em um dia) x 730 horas em um mês = 686.2000 USD
	   
	30 GB por mês x 0,437 USD x 1 instâncias = 13,11 USD (Custo de armazenamento)<br>
	Preço do armazenamento (mensal): **13.11 USD**<br>
	Custo mensal total: **1,385.51 USD**

3. **Amazon Textract**:
   - O **Amazon Textract** é um serviço de **machine learning (ML)** que extrai automaticamente texto, escrita à mão e dados de documentos digitalizados. Ele vai além do simples reconhecimento óptico de caracteres (OCR) para identificar, compreender e extrair dados de formulários e tabelas. Com o Textract, você paga apenas pelo que utiliza, sem taxas mínimas ou compromissos iniciais. O custo do Textract depende do número de páginas processadas.
   - O custo do Textract depende da quantidade de páginas processadas e do uso de recursos adicionais, como análise de formulários.
 
Para estimar o custo de **3000 páginas** com tabelas, formulários e consultas, considere o seguinte:

- **Preço por página com Tabelas, Formulários e Consultas**:
  - **Primeiro milhão de páginas**: $0,070 por página.
  - **Próximo milhão de páginas**: $0,055 por página.
  - **Custo total** = ($0,070 * 3.000) = **$210.00 USD**.


## Conclusão
Custo inicial: $0,00 USD <br>
Custo mensal: $1599.4 USD<br>
Custo total de 12 months: $19192.8 USD


Assinatura do Responsável pelo Projeto:

Victor Sérgio Silva Barros