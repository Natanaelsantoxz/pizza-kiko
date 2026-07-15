# Site — Yasmin Moreira | Especialista em Cachos e Ondulados

Site institucional de uma página (one-page), pronto para publicar no GitHub Pages.

## Estrutura
```
index.html     -> conteúdo do site
styles.css     -> visual (cores, tipografia, layout)
script.js      -> menu mobile, animações de rolagem
assets/
  favicon.svg  -> ícone da aba do navegador
```

## Sobre as fotos e vídeos
Não foi possível copiar fotos ou vídeos reais do perfil do Instagram
(@yasminjmoreira) para dentro do site — perfis do Instagram são fechados
para esse tipo de extração automática, e usar fotos de terceiros sem
permissão explícita também não seria correto.

Em vez disso, o site tem:
- Espaços reservados (placeholders) nas seções **Sobre** e **Galeria**,
  já no tamanho e formato certos — é só trocar pela imagem real.
- Botões destacados de **"Saiba mais no Instagram"** que levam direto para
  https://www.instagram.com/yasminjmoreira

### Como trocar um placeholder por uma foto real
1. Coloque o arquivo da foto dentro da pasta `assets/` (ex: `assets/foto-sobre.jpg`).
2. Na seção "Sobre" do `index.html`, troque o bloco `<svg class="portrait-placeholder">...` por:
   ```html
   <img src="assets/foto-sobre.jpg" alt="Yasmin Moreira" class="portrait-placeholder" style="object-fit:cover;">
   ```
3. Na "Galeria", cada `<div class="galeria-item ph-1">` pode virar:
   ```html
   <div class="galeria-item">
     <img src="assets/galeria-1.jpg" alt="Transformação de cacho" style="width:100%;height:100%;object-fit:cover;">
   </div>
   ```

## Como publicar no GitHub Pages
1. Crie um repositório novo no GitHub (ex: `yasmin-moreira-site`).
2. Envie todos os arquivos deste ZIP para a raiz do repositório.
3. No repositório, vá em **Settings → Pages**.
4. Em "Source", selecione a branch `main` e a pasta `/ (root)`.
5. Salve. Em alguns minutos o site estará no ar em:
   `https://SEU-USUARIO.github.io/yasmin-moreira-site/`

## Personalizar textos
Todos os textos (serviços, depoimentos, bio) estão em português dentro do
`index.html` e podem ser editados livremente — são só um ponto de partida
profissional para você ajustar com os detalhes reais do atendimento.
