# Classificação e Segmentação de Documentos Brasileiros com Redes Neurais

Este repositório apresenta uma solução baseada em redes neurais convolucionais (CNNs) e U-Net para classificação automática de tipos de documentos brasileiros e segmentação visual de seus contornos. O sistema pode ser executado diretamente via Google Colab, sem necessidade de instalação local.

---

## 🚀 Funcionalidades

- **Classificação de documentos** (RG, CNH, CPF etc.) usando uma CNN treinada do zero.
- **Segmentação de documentos** em imagens usando a arquitetura U-Net.
- **Execução via Google Colab**, com exemplos prontos para uso e visualização de resultados.

---

## ▶️ Como Executar o Projeto

### 3. Passo a Passo (dentro do Colab)

1. Acesse o notebook que deseja utilizar:
   - [Classificação de Documentos](https://colab.research.google.com/drive/1M4lEvT313MepnpC1xiNOJ6JVMONpvKFd?usp=sharing)
   - [Segmentação de Documentos](https://colab.research.google.com/drive/1XZ0y2ZRSvIn-6lVXbkcWb1_6pezEvAvb?usp=sharing)

2. Os notebooks estão preparados para funcionar com os caminhos e estrutura dos dois datasets utilizados neste projeto.

3. Antes de executar, verifique se você está utilizando os mesmos conjuntos de dados ou estruturas compatíveis. Caso esteja usando arquivos em outro local do Drive ou um dataset diferente, será necessário substituir os caminhos no código de acordo com sua organização de pastas.  
Os caminhos no código estão definidos de forma genérica (como `/caminho/para/sua/pasta/...`), então você deve ajustá-los para refletir corretamente onde seus arquivos estão armazenados.

4. O projeto assume a seguinte estrutura de arquivos:
   - Imagens organizadas por classe (no caso do BID)
   - Máscaras de segmentação correspondentes (no caso do SpotBID)
   - Pastas separadas para treino e validação
   - Diretórios definidos para salvar modelos e checkpoints

A estrutura foi pensada especificamente para funcionar com os datasets descritos abaixo.

---

### 📦 Datasets utilizados

- **Brazilian Identity Document Dataset (BID)** — usado na parte de classificação  
  🔗 https://github.com/ricardobnjunior/Brazilian-Identity-Document-Dataset  
  Contém imagens reais de documentos brasileiros (RG, CNH, CPF etc.), organizadas por classe em pastas distintas.

- **SpotBid-Set Dataset** — usado na parte de segmentação  
  🔗 https://github.com/ricardobnjunior/SpotBid-Set-Dataset  
  Contém imagens e suas respectivas máscaras de segmentação que indicam os contornos visuais dos documentos.

⚠️ **Importante**: caso decida utilizar outros conjuntos de dados, será necessário ajustar a estrutura de diretórios, formatos de entrada e possivelmente o código de carregamento para que tudo funcione corretamente.


