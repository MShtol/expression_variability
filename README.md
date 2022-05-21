# Dissecting the role of gene expression variability in complex traits

Genome-Wide Association Study (GWAS) is a technique used to look for genome sequence variations that affect the development of complex traits. In recent years, GWAS results have been published for thousands of different traits, including two of the world's largest datasets, UK Biobank and Finngen. It is known that changes in gene expression levels are one of the main mechanisms that determine the small effects of genetic variants detected during GWAS. In this project, we test the hypothesis that not only the level of gene expression, but also the degree of expression variability, is associated with the influence of a gene on complex human traits.

## Reqierements and tools
In this project Python=3.8 was udes with tje following packages:

In this project both Plink 1.9 and Plink 2.0. You can install from bioconda with following:

`conda install -c bioconda plink`

`conda install -c bioconda plink2`

If you don't have Conda, install it first.


## Gtex

wget https://storage.googleapis.com/gtex_analysis_v8/rna_seq_data/GTEx_Analysis_2017-06-05_v8_RNASeQCv1.1.9_gene_tpm.gct.gz


## GWAS
Donwload and unpack:

wget https://broad-ukb-sumstats-us-east-1.s3.amazonaws.com/round2/additive-tsvs/4194_irnt.gwas.imputed_v3.both_sexes.tsv.bgz -O 4194_irnt.gwas.imputed_v3.both_sexes.tsv.gz
wget https://broad-ukb-sumstats-us-east-1.s3.amazonaws.com/round2/annotations/variants.tsv.bgz -O variants.tsv.gz
gunzip /pulse_rate/*.gz
paste -d, ./pulse_rate/variants.tsv ./pulse_rate/4194_irnt.gwas.imputed_v3.both_sexes.tsv > 4194_irnt.gwas.imputed_v3.both_sexes_merged.tsv


2. Отчет по результатам работы над проектом (репозиторий)

Весь проект оформляется на английском языке;
Все результаты должны быть оформлены на GitHub:
для вашей НИР вы создаете отдельный проект и, если вас в группе несколько человек, добавляете остальных в коллабораторы;
репозиторий должен быть публичным;
если работа ведется над чужим закрытым кодом, выложите только ту часть, над которой работали непосредственно вы (с разрешения руководителя);
в проекте должен содержаться файле README.md, содержащий следующие основные элементы:
цели и задачи проекта;
результаты, сопровождаемые иллюстрациями;
сделанные выводы;
ссылки на используемую литературу, базы данных и пр.
Если проект направлен на создание ПО:
выложенный в репозитории код должен быть сопровожден содержательными комментариями;
должны быть прописаны системные требования (по памяти/CPU, необходимая версия операционной системы, интерпретатора, библиотек и пр.);
примеры получаемых результатов (текст, графики, таблицы и пр.) и входных данных (таблицы, тексты).
Если проект направлен на использование уже разработанных программ, необходимо включить:
краткое описание используемых методов;
версии программ и команды запуска со всеми параметрами;
комментарии, почему были выбраны именно такие параметры.



## Reference

