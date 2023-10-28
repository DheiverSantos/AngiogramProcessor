# Processamento de Imagens de Angiograma com Python

Este script em Python demonstra como processar imagens de angiograma usando a biblioteca OpenCV. Imagens de angiograma são comumente usadas em imagens médicas para visualizar vasos sanguíneos, particularmente no contexto da angiografia coronária.

## Como o Código Funciona

1. **Importação de Bibliotecas**: O código começa importando as bibliotecas necessárias:
   - `cv2` para operações de visão computacional
   - `numpy` para cálculos numéricos
   - `matplotlib` para visualização de imagens

2. **Definição da Classe - `AngiogramProcessor`**:
   - A classe `AngiogramProcessor` é definida para encapsular a funcionalidade de processamento de imagens.
   - Ela é inicializada com o caminho para uma imagem de angiograma.

3. **Passos de Processamento de Imagem**:
   - O método `load_image` carrega a imagem do angiograma.
   - O método `convert_to_grayscale` converte a imagem para escala de cinza.
   - O método `equalize_histogram` melhora o contraste da imagem usando equalização de histograma.
   - O método `smooth_image` aplica suavização Gaussiana para reduzir ruídos.
   - O método `threshold_and_process` cria uma máscara binária dos vasos sanguíneos usando limiar adaptativo.

4. **Visualização de Imagens**:
   - O método `show_original_image` exibe a imagem original do angiograma.
   - O método `show_veins_mask` exibe a máscara binária dos vasos sanguíneos.

5. **Análise de Componentes Conectados**:
   - O método `keep_connected_components` mantém apenas os maiores componentes conectados na máscara de vasos.
   - Ele utiliza análise de componentes conectados para identificar e manter as estruturas vasculares significativas.

6. **Processamento e Exibição**:
   - O método `process_and_show` orquestra toda a sequência de processamento de imagens.
   - Ele exibe tanto a imagem original quanto a máscara de vasos processada lado a lado.

7. **Exemplo de Uso**:
   - No exemplo fornecido, uma imagem de angiograma é carregada, processada e exibida usando a classe `AngiogramProcessor`.

## Por que Este Código é Útil

- Este código é útil para processamento de imagens médicas, especialmente no contexto de angiografia.
- Ele permite a visualização e análise de vasos sanguíneos em imagens de angiograma.
- O código melhora a qualidade da imagem, remove ruídos e destaca as estruturas vasculares.

## Como Usar Este Código

1. Substitua `image_path` pelo caminho para sua própria imagem de angiograma.
2. Personalize os parâmetros de processamento conforme necessário.
3. Execute o script para visualizar a imagem original e a máscara de vasos.
4. Ajuste os limiares de limite e os limiares de tamanho dos componentes conectados para suas imagens específicas.
5. Integre este código em projetos maiores para análise automatizada de angiogramas.

Este projeto é mantido pelo Dr. Dheiver Francisco Santos, da Genius AI. Para obter mais informações sobre o autor, visite [LinkedIn](https://www.linkedin.com/in/dheiver-santos) ou envie um email para [dheiver.santos@gmail.com](mailto:dheiver.santos@gmail.com).
