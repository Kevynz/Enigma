# Caça ao Tesouro Bíblico - Igreja Pentecostal

## 📋 Descrição do Projeto

Este é um sistema de caça ao tesouro bíblico desenvolvido para igrejas pentecostais com foco em **trabalho em equipe**. Os participantes visitam diferentes locais da igreja, resolvem charadas bíblicas sobre colaboração cristã e coletam palavras que formam uma frase final sobre unidade na igreja.

**Tradução Bíblica Utilizada:** Almeida Revista e Corrigida (ARC)

## 🏛️ Locais e Charadas - TEMA: TRABALHO EM EQUIPE

### 1. **🎤 Púlpito** (`pulpito.html`)
- **Função**: Local onde se proclama a Palavra de Deus
- **Charada**: Sobre o corpo de Cristo e unidade
- **Resposta**: 1Co(12:27) 4 = "corpo"
- **Versículo**: "Ora, vós sois o corpo de Cristo, e seus membros em particular." (ARC)

### 2. **✝️ Altar** (`altar.html`)
- **Função**: Local de oração, consagração e entrega
- **Charada**: Sobre viver em harmonia
- **Resposta**: 1Co(1:10) 4 = "sejais"
- **Versículo**: "Rogo-vos, pois, irmãos, pelo nome de nosso Senhor Jesus Cristo, que sejais todos unidos no falar e no sentir, e que não haja entre vós dissensões; antes sejais unidos em um mesmo parecer e em um mesmo propósito." (ARC)

### 3. **💧 Batistério** (`batisterio.html`)
- **Função**: Onde pessoas nascem de novo
- **Charada**: Sobre nossa união em Cristo
- **Resposta**: Rm(12:5) 6 = "corpo"
- **Versículo**: "Assim nós, que somos muitos, somos um só corpo em Cristo, mas individualmente somos membros uns dos outros." (ARC)

### 4. **🚪 Entrada Principal** (`entrada.html`)
- **Função**: Local por onde todos entram na casa do Senhor
- **Charada**: Sobre cuidado mútuo
- **Resposta**: 1Co(12:25) 6 = "cuidado"
- **Versículo**: "Para que não haja divisão no corpo, mas que os membros tenham igual cuidado uns dos outros." (ARC)

### 5. **📚 Biblioteca** (`biblioteca.html`)
- **Função**: Local onde se estuda e busca conhecimento
- **Charada**: Sobre edificar uns aos outros
- **Resposta**: Rm(15:2) 10 = "bom"
- **Versículo**: "E que cada um de nós agrade ao seu próximo no que é bom para edificação." (ARC)

### 6. **👶 Salão Infantil** (`salaoinfantil.html`)
- **Função**: Local onde se ensina as crianças sobre Jesus
- **Charada**: Sobre ajudar no fardo do próximo
- **Resposta**: Gl(6:2) 6 = "cumprireis"
- **Versículo**: "Levai as cargas uns dos outros, e assim cumprireis a lei de Cristo." (ARC)

### 7. **📋 Secretaria** (`secretaria.html`)
- **Função**: Local onde se organiza e administra a igreja
- **Charada**: Sobre administrar os dons
- **Resposta**: 1Pe(4:10) 13 = "despenseiros"
- **Versículo**: "Cada um administre aos outros o dom como o recebeu, como bons despenseiros da multiforme graça de Deus." (ARC)

### 8. **🌻 Jardim** (`jardim.html`)
- **Função**: Local que mostra a criação e beleza de Deus
- **Charada**: Sobre sermos construção divina
- **Resposta**: 1Co(3:9) 9 = "edifício"
- **Versículo**: "Porque somos cooperadores de Deus; vós sois lavoura de Deus, edifício de Deus sois." (ARC)

## 📖 Sistema de Codificação

O formato de resposta segue o padrão: **Livro(capítulo:versículo) número_da_palavra**

### Exemplos:
- `Gn(12:3) 2` = Gênesis, capítulo 12, versículo 3, segunda palavra
- `Mt(5:14) 1` = Mateus, capítulo 5, versículo 14, primeira palavra

### Abreviações dos Livros Bíblicos Utilizadas:
- **1Co** = 1 Coríntios
- **Rm** = Romanos
- **Gl** = Gálatas
- **1Pe** = 1 Pedro

## 🔧 Implementação dos QR Codes

### Passo 1: Gerar os QR Codes
Para cada página, você precisa gerar QR codes que apontem para as URLs das páginas:

```
https://seudominio.com/pulpito.html
https://seudominio.com/altar.html
https://seudominio.com/batisterio.html
https://seudominio.com/entrada.html
https://seudominio.com/biblioteca.html
https://seudominio.com/salaoinfantil.html
https://seudominio.com/secretaria.html
https://seudominio.com/jardim.html
```

### Passo 2: Criar a pasta de imagens
Crie uma pasta chamada `qr-codes` na raiz do projeto.

### Passo 3: Adicionar as imagens
Salve os QR codes gerados com os seguintes nomes:
- `pulpito-qr.png`
- `altar-qr.png`
- `batisterio-qr.png`
- `entrada-qr.png`
- `biblioteca-qr.png`
- `salaoinfantil-qr.png`
- `secretaria-qr.png`
- `jardim-qr.png`

### Passo 4: Descomentarizar o código HTML
Em cada arquivo HTML, localize esta seção:
```html
<!-- <div class="qr-code">
    <img src="qr-codes/[nome]-qr.png" alt="QR Code do [Local]" style="width: 150px; height: 150px;">
</div> -->
```

E remova os comentários:
```html
<div class="qr-code">
    <img src="qr-codes/[nome]-qr.png" alt="QR Code do [Local]" style="width: 150px; height: 150px;">
</div>
```

### Ferramentas para gerar QR Codes:
- **Online**: QR Code Generator, qr-code-generator.com
- **Programático**: Biblioteca qrcode (Python), qr-server API
- **Apps**: QR Code Generator (mobile)

## 🎯 Como Usar

1. **Preparação**: Coloque QR codes ou imprima as charadas em cada local da igreja
2. **Instrução**: Explique aos participantes o formato das respostas
3. **Execução**: Os participantes visitam os locais, resolvem as charadas e anotam as respostas
4. **Finalização**: Verificam a solução final na página `solucao.html`

## 🌟 Frase Final Formada - TRABALHO EM EQUIPE

Coletando todas as palavras na ordem dos locais:
**"Corpo sejais corpo cuidado bom cumprireis despenseiros edifício"**

Esta sequência ensina sobre colaboração cristã:
- **Corpo** - Somos um só corpo em Cristo
- **Sejais** - Chamado à unidade  
- **Corpo** - Reforça nossa união
- **Cuidado** - Cuidado mútuo entre irmãos
- **Bom** - O que é edificante
- **Cumprireis** - Ação de completar/realizar
- **Despenseiros** - Administradores dos dons
- **Edifício** - Construção conjunta da igreja

**Mensagem Final:** *"Sejam um só corpo, tenham cuidado uns dos outros, façam o bem, cumpram a lei de Cristo, sejam bons administradores e construam juntos o edifício de Deus!"*

## 🔄 Personalização

Você pode facilmente:
- Modificar as charadas para adequar à sua igreja
- Alterar os locais conforme sua estrutura física  
- Ajustar as referências bíblicas
- Personalizar cores e estilos no CSS
- Adicionar mais locais ou reduzir conforme necessário

## 📱 Compatibilidade

- Design responsivo para celulares e tablets
- Funciona em todos os navegadores modernos
- Não requer internet após carregamento inicial
- Interface intuitiva e amigável