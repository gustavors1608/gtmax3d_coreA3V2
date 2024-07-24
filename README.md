# GTMax3D Core A3 V2 - Documentação

Bem-vindo à documentação da impressora 3D GTMax3D modelo Core A3 V2. Este repositório contém todas as informações necessárias para configurar e operar a impressora, incluindo perfis de materiais, configuração de bicos, tamanho da mesa, scripts e arquivos G-code testados.

## Tipos de Filamentos: Vantagens e Desvantagens e qual escolher em cada ocasião

### ABS (Acrilonitrila Butadieno Estireno)

#### Vantagens:
- **Resistência ao Calor**: O ABS tem alta resistência ao calor, tornando-o adequado para peças que podem ser expostas a altas temperaturas.
- **Durabilidade**: É conhecido por sua alta resistência ao impacto, sendo ideal para peças que precisam ser fortes e duráveis.
- **Flexibilidade**: Embora não seja tão flexível quanto alguns outros filamentos, o ABS tem alguma flexibilidade, o que pode ser benéfico para certas aplicações.

#### Desvantagens:
- **Emissão de Fumos**: Durante a impressão, o ABS pode liberar fumos que podem ser irritantes. É recomendável imprimir em uma área bem ventilada.
- **Encolhimento e Deformação**: O ABS tende a encolher à medida que esfria, o que pode levar à deformação (warping) das peças. A utilização de uma mesa aquecida e técnicas como raft ou brim podem ajudar a minimizar esses problemas.
- **Adesão à Mesa**: Pode ser difícil obter uma boa adesão inicial à mesa de impressão sem uma preparação adequada.

### PLA (Ácido Poliláctico)

#### Vantagens:
- **Fácil de Imprimir**: O PLA é considerado um dos filamentos mais fáceis de imprimir, com menor risco de deformação e encolhimento.
- **Biodegradável**: Feito de recursos renováveis como amido de milho, o PLA é mais ecológico do que muitos outros tipos de filamento.
- **Menor Emissão de Fumos**: Em comparação com o ABS, o PLA emite menos fumos durante a impressão, tornando-o mais seguro para uso em ambientes fechados.

#### Desvantagens:
- **Resistência ao Calor**: O PLA tem baixa resistência ao calor e pode deformar-se em temperaturas relativamente baixas (acima de 60°C).
- **Fragilidade**: Embora seja forte, o PLA é mais frágil e menos resistente ao impacto em comparação com o ABS e outros filamentos.
- **Degradação ao Longo do Tempo**: Em condições específicas, o PLA pode degradar-se mais rapidamente do que outros materiais.

### PETG (Polietileno Tereftalato Glicol)

#### Vantagens:
- **Combinação de Rigidez e Flexibilidade**: O PETG oferece uma boa combinação de rigidez e flexibilidade, tornando-o adequado para uma ampla gama de aplicações.
- **Fácil Adesão e Menor Deformação**: O PETG adere bem à mesa de impressão e tem menor risco de deformação em comparação com o ABS.
- **Resistência Química**: O PETG é resistente a muitos produtos químicos, incluindo ácidos e álcalis.

#### Desvantagens:
- **Stringing**: O PETG pode ser propenso a stringing (filamentos finos entre as partes impressas) se as configurações de retração não forem ajustadas corretamente.
- **Transparência**: Embora a transparência possa ser uma vantagem em algumas aplicações, ela pode não ser desejada para todas as peças.
- **Temperatura de Impressão**: Requer temperaturas de impressão mais altas, o que pode não ser adequado para todas as impressoras.

### Tritan

#### Vantagens:
- **Alta Resistência ao Impacto**: O Tritan é extremamente resistente ao impacto, tornando-o ideal para peças que precisam suportar forças significativas.
- **Resistência ao Calor**: Este material mantém suas propriedades mecânicas em temperaturas mais altas, adequado para aplicações que exigem resistência ao calor.
- **Durabilidade e Estabilidade Dimensional**: O Tritan oferece alta durabilidade e estabilidade dimensional, sendo ideal para peças precisas e duradouras.

#### Desvantagens:
- **Dificuldade de Impressão**: Pode ser mais difícil de imprimir do que PLA e PETG, exigindo configurações de impressão específicas.
- **Custo**: Geralmente, o Tritan é mais caro do que outros filamentos como PLA e ABS.
- **Adesão à Mesa**: Pode ser necessário utilizar adesivos especiais ou superfícies de impressão para garantir uma boa adesão inicial.

---

Cada tipo de filamento tem suas próprias vantagens e desvantagens, e a escolha do material adequado depende das necessidades específicas do seu projeto. Certifique-se de ajustar as configurações da impressora para otimizar a qualidade da impressão de acordo com o material escolhido.

## Configuração de Materiais

### ABS

- **Temperatura do bico**: 240-250°C
- **Temperatura da mesa**: 100-110°C
- **Velocidade de impressão**: 40-60 mm/s
- **Configuração do perfil**: [Download do perfil ABS](https://github.com/gustavors1608/gtmax3d_coreA3V2/blob/main/config/Cura%20ABS%20Bico%200.5.curaprofile)

### PLA

- **Temperatura do bico**: 190-210°C
- **Temperatura da mesa**: 50-60°C
- **Velocidade de impressão**: 60-80 mm/s
- **Configuração do perfil**: [Download do perfil PLA](https://github.com/gustavors1608/gtmax3d_coreA3V2/blob/main/config/Cura%20PLA%20Bico%200.5.curaprofile)

### PETG

- **Temperatura do bico**: 230-250°C
- **Temperatura da mesa**: 70-80°C
- **Velocidade de impressão**: 50-70 mm/s
- **Configuração do perfil**: [Download do perfil PETG](https://github.com/gustavors1608/gtmax3d_coreA3V2/blob/main/config/Cura%20PETG%20Bico%200.5.curaprofile)

### Tritan

- **Temperatura do bico**: 250-270°C
- **Temperatura da mesa**: 100-110°C
- **Velocidade de impressão**: 40-60 mm/s
- **Configuração do perfil**: [Download do perfil Tritan](https://github.com/gustavors1608/gtmax3d_coreA3V2/blob/main/config/Cura%20Tritan%20Bico%200.5.curaprofile)

## Configuração do Bico e da Mesa

### Visão Geral da Impressora / Mesa

![Impressora A3V2](https://github.com/gustavors1608/gtmax3d_coreA3V2/blob/main/config/Impressora%20A3V2.jpg)

### Visão Geral do Extrusor / Bico

![Extruder A3V2](https://github.com/gustavors1608/gtmax3d_coreA3V2/blob/main/config/Extruder%20A3V2.jpg)

### Scripts para Mesa e Bico

- Atenção: o script dos 2 itens está no mesmo arquivo. É necessário copiar somente a parte do extrusor na parte de configuração do extrusor (sessão "Visão Geral do Extrusor / Bico") e o mesmo para a mesa de impressão.
- **Configuração**: [Download do script de configuração](https://github.com/gustavors1608/gtmax3d_coreA3V2/blob/main/config/SCRIPT%20CURA%20A3V2.txt)

## Arquivos G-code

- [G-code testado para ABS (benchy)](https://github.com/gustavors1608/gtmax3d_coreA3V2/blob/main/config/3DBenchy.gcode)
- G-code testado para PLA -> não testado por falta de filamento
- G-code testado para PETG -> não testado por falta de filamento
- G-code testado para Tritan -> não testado por falta de filamento

## Explicações Técnicas

### Z-offset

O **Z-offset** é a distância entre a ponta do bico e a superfície da mesa de impressão quando o bico está na posição inicial (home). Essa medida é crucial para garantir que a primeira camada do material adira corretamente à mesa. A unidade de medida do Z-offset é milímetros (mm). Por exemplo, um valor de Z-offset de 3,450 mm significa que a ponta do bico está a 3,450 mm acima da superfície da mesa na posição inicial.

**Influência do Z-offset**:
- Um Z-offset muito baixo pode causar entupimentos no bico e danos à mesa.
- Um Z-offset muito alto pode resultar em má adesão da primeira camada, comprometendo a qualidade da impressão.

### Temperatura do Bico vs Velocidade

A **temperatura do bico** e a **velocidade de impressão** são parâmetros interdependentes. Uma temperatura mais alta permite uma impressão mais rápida, pois o material é extrudido de maneira mais eficiente. No entanto, uma temperatura muito alta pode causar problemas como stringing (filamentos finos entre as partes impressas) e deformação. É importante encontrar um equilíbrio para cada

 tipo de material.

**Considerações**:
- Materiais como ABS e Tritan requerem temperaturas de bico mais altas e, consequentemente, podem suportar velocidades de impressão mais baixas para evitar deformações.
- O PLA pode ser impresso a temperaturas mais baixas e em velocidades mais altas, mas um resfriamento adequado é crucial para evitar deformações.

### Temperatura da Mesa vs Adesão do Material

A **temperatura da mesa** é crucial para a adesão do material à superfície de impressão. Materiais como ABS e Tritan requerem uma mesa aquecida a temperaturas mais altas para evitar o warping (deformação), enquanto o PLA pode ser impresso a temperaturas de mesa mais baixas. A correta temperatura da mesa garante uma boa adesão da primeira camada, o que é essencial para uma impressão bem-sucedida.

**Influência da Temperatura da Mesa**:
- Alta temperatura da mesa melhora a adesão inicial, mas pode causar deformações se for muito alta.
- Temperaturas baixas podem resultar em falhas de adesão e descolamento durante a impressão.

### Retract

O **retract** (retração) é a ação de puxar o filamento de volta para dentro do bico antes de se mover para uma nova posição, a fim de evitar o stringing e vazamentos. Ajustes finos na configuração de retração podem melhorar significativamente a qualidade da impressão.

**Configurações de Retract**:
- **Distância de retração**: A quantidade de filamento retraído.
- **Velocidade de retração**: A rapidez com que o filamento é retraído.

### Flow Rate

O **flow rate** (taxa de fluxo) refere-se à quantidade de filamento extrudido pelo bico. Ajustes na taxa de fluxo podem corrigir problemas de subextrusão (muito pouco material) ou sobreextrusão (muito material).

### Cooling

O **cooling** (resfriamento) é crítico para a solidificação correta do material extrudido. Ventiladores de resfriamento podem ser ajustados para garantir que o material solidifique rapidamente, minimizando deformações e melhorando a precisão dos detalhes.

**Configurações de Resfriamento**:
- **Velocidade do ventilador**: Ajustável para diferentes materiais e geometrias.
- **Tempo de resfriamento**: Importante para camadas finas e detalhes complexos.

### Raft

O **raft** é uma base de suporte impressa sob a peça principal. Ele melhora a adesão à mesa e ajuda a evitar deformações, especialmente em materiais mais difíceis de imprimir. O raft é removido após a impressão.

**Vantagens**:
- Melhora a adesão inicial.
- Facilita a remoção da peça da mesa.

### Brim

O **brim** é uma borda fina e ampla ao redor da base da peça. Ele aumenta a área de contato com a mesa, melhorando a adesão inicial e ajudando a evitar warping. Diferente do raft, o brim é geralmente mais fácil de remover e usa menos material.

**Vantagens**:
- Melhora a adesão inicial.
- Fácil de remover e consome menos material que o raft.

## Dicas Extra

**Caso não estiver grudando a peça na mesa**
- Usar uma camada de cola de EVA/isopor no local onde será impressa a peça. Passe antes de aquecer a mesa, aplique em um local e espalhe com o dedo, espátula, etc.
- Outra opção é aumentar o fluxo de material na sessão de ajustes finos da impressora (geralmente valores de 150 (150%) resolvem), isso fará a primeira camada ter muito mais material e ficar mais compactada contra a mesa. Lembre-se de voltar o valor para 100 após imprimir a primeira camada.
- Caso ainda assim não grude, é possível utilizar o recurso "raft" no software de fatiamento, talvez usar em conjunto com as dicas anteriores.
- Modo extremo: algumas gotas de super bonder (usar bem pouco durante a impressão da primeira camada). Porém, tenha cuidado ao retirar e, após a impressão, limpe o vidro para não deixar resíduos que possam atrapalhar as próximas impressões.

## Vídeos Tutoriais

### Verificando o Acionamento do Sensor - Parte 1 (em caso de problema)

![Verificando acionamento sensor - Parte 1](https://github.com/gustavors1608/gtmax3d_coreA3V2/blob/main/config/1%C2%B0%20Verificando%20acionamento%20sensor.mp4)

### Verificando o Acionamento do Sensor - Parte 2 (em caso de problema)

![Verificando acionamento sensor - Parte 2](https://github.com/gustavors1608/gtmax3d_coreA3V2/blob/main/config/2%C2%B0%20Verificando%20acionamento%20sensor.mp4)

### Carregando Configurações para o Cura

![Carregando configurações para o Cura](https://github.com/gustavors1608/gtmax3d_coreA3V2/blob/main/config/Carregando%20configura%C3%A7%C3%B5es%20para%20o%20Cura.mp4)

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para me chamar e tirar dúvidas ou sugerir melhorias.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).
