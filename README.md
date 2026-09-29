# 🛍️ Catálogo Digital Artesane 3D

Catálogo responsivo interativo para seleção de produtos personalizados e envio direto de pedidos via WhatsApp.

---

## 📸 Como adicionar mais fotos a um produto

No arquivo [`index.html`](file:///c:/Users/armando.lemos/Documents/Sistemas/CatalogoArtesane/index.html), localize a constante `products` no script.

Cada produto agora possui o campo `images` configurado como uma lista (`array`). Você pode adicionar quantas fotos desejar:

```javascript
{ 
    id: "01", 
    category: "Chaveiros", 
    icon: "🔑", 
    name: "Chaveiro de Nome Colorido", 
    desc: "Placa em 2 cores vibrantes com corrente e argola de metal super resistente.", 
    priceUnit: 10.0, 
    priceBulk: 6.0, 
    images: ["01.jpg", "01_detalhe.jpg", "01_cores.jpg"] // 👈 Adicione os nomes dos arquivos aqui
}
```

Basta salvar as fotos na mesma pasta do repositório (ex: `01_detalhe.jpg`) e adicioná-las ao Git:

```bash
git add .
git commit -m "Adiciona fotos adicionais aos produtos"
git push
```

---

## ✨ Principais Melhorias Implementadas

1. **Galeria Multi-foto e Modal Lightbox**:
   - Cada card possui navegação com setas e indicadores para alternar fotos.
   - Ao clicar na foto, abre-se uma tela cheia (*lightbox*) com zoom e miniaturas na parte inferior.
   - Navegação por teclado com setas e tecla `ESC`.
2. **Design Visual Moderno & Premium**:
   - Tipografia integrada com **Plus Jakarta Sans** e **Outfit**.
   - Gradientes vibrantes, cantos arredondados modernos e microinterações táteis.
   - Destaque em amarelo/laranja e verde com contraste calibrado.
3. **Filtro por Categorias e Barra de Busca**:
   - Botões estilo pílula (*chips*) para filtrar categorias (Chaveiros, Marcadores, Tags, etc.).
   - Campo de busca instantâneo por nome ou código do item.
4. **Calculadora e Regra de Atacado em Tempo Real**:
   - Aplicação automática do preço de atacado para 10 ou mais unidades.
   - Atualização visual instantânea nos cards e no resumo inferior.
5. **Barra Fixa Flutuante & Mensagem WhatsApp Formatada**:
   - Barra inferior com efeito vidro (*glassmorphism*) que não tampa os botões.
   - Mensagem clara, organizada com emojis, subtotais e identificação de atacado.
