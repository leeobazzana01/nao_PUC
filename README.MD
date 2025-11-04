# MATRIZ DAS CAPACIDADES OPERACIONAIS NAO

Implementação de uma Matriz das Capacidades Operantes na Plataforma NAO.


## Participantes 
1. Diego Oliveira Peixoto
2. FLávio de Lima e Silva Neto
3. Leonardo José Bazana Lima
4. Pedro de Mello Camargo

**Disciplina: Robôs, Sensores e Aplicações - Ciência da Computação**
**Professor: Harison Herman**

## 1. RESUMO

A utilização de robôs humanoides como assistentes virtuais em ambientes educacionais é o presente e também o futuro, representando uma fronteira inovadora para a melhoria de serviços institucionais. Plataformas como o robô NAO demonstram potencial para atuar como facilitadores de acesso à informação. A adoção das tecnologias robóticas na instituição, obtidas através de parcerias com a iniciativa privada, enfrenta algumas dificuldades principais: (1) ausência de informações quanto às versões específicas da plataforma; e (2) incerteza quanto ao estado funcional, o que poderia inviabilizar projetos devido a questões operacionais. Este artigo propõe uma metodologia dupla: (1) verificação da versão específica do robô NAO disponível para uso na universidade, seguindo as diretrizes da documentação oficial; e (2) uma metodologia de revisão e validação sistemática (V&V), utilizando a documentação oficial “Alderbaran Documentation” para avaliar quais funcionalidades estão operantes. O objetivo do estudo é desenvolver uma matriz de capacidades operacionais do NAO e as possíveis limitações impostas por componentes inoperantes. Os resultados buscam demonstrar a viabilidade técnica da plataforma, propondo um panorâma geral de possíveis integrações a sererm feitas para realizar tarefas na Universidade.  

Palavras-chave: *Robótica. NAO. Verificação e Validação.* 

## ABSTRACT

The use of humanoid robots as virtual assistants in educational environments represents both the present and the future, marking an innovative frontier for enhancing institutional services. Platforms such as the NAO robot demonstrate strong potential as facilitators of information access. The adoption of robotic technologies within academic institutions—often made possible through partnerships with private initiatives—faces key challenges: (1) the lack of detailed information regarding specific platform versions, and (2) uncertainty about the robot’s functional state, which can hinder project development due to operational issues. This paper proposes a dual methodology: (1) verifying the specific version of the NAO robot available for use at the university, following the official documentation guidelines; and (2) applying a systematic verification and validation (V&V) process based on the Aldebaran Documentation to assess which functionalities are currently operational. The goal of this study is to develop a matrix of the NAO robot’s operational capabilities and identify potential limitations imposed by non-functional components. 

Keywords: *Robotics. NAO. Verification and Validation.* 

## 2. INTRODUÇÃO

### 2.1 Contextualização

A robótica de serviço tem avançado significativamente como ferramenta de suporte em ambientes institucionais, onde robôs como o NAO podem atuar como assistentes virtuais em diversas tarefas da Universidade, promovendo o acesso democratizado à informação e reduzindo a carga sobre equipes administrativas. Em instituições educacionais, essa tecnologia representa uma oportunidade para otimizar processos e melhorar a experiência do aluno. 

### 2.2 Problema de Pesquisa

A implementação dessas tecnologias enfrenta desafios específicos relacionados à falta de informações técnicas detalhadas sobre as versões da plataforma bem como ao estado funcional dos componentes. Essa incerteza pode resultar em significativos investimentos de tempo em debugging e, em casos extremos, inviabilizar projetos promissores. 

### 2.3 Objetivos

**Objetivo Principal:** Propor e aplicar uma metodologia de verificação e validação (V&V) para o robô NAO e, com base nos resultados obtidos, avaliar a viabilidade de uso da plataforma a serviço da Instituição. 

### 3 FUNDAMENTAÇÃO TEÓRICA 

#### 3.1 O Robô NAO e a Plataforma NAOqi 

O robô NAO, desenvolvido pela Aldebaran Robotics (atualmente SoftBank Robotics), constitui uma plataforma humanóide amplamente utilizada em pesquisa, educação e aplicações variadas. A arquitetura do NAO inclui múltiplos sensores, atuadores e sistemas de percepção que permitem interações complexas com o ambiente. A plataforma NAOqi fornece uma API abrangente para programação e controle dos diversos subsistemas do robô. 

#### 3.2 Especificações Técnicas e Identificação de Versões 

A identificação precisa da versão do hardware e software do NAO é essencial. Existem diferentes gerações do robô (como NAO V5, V6) e versões do NAOqi (API) possuem capacidades distintas e compatibilidades que variam. A documentação oficial fornece protocolos específicos para identificação dessas versões através de interfaces físicas e software. 

#### 3.3 Verificação e Validação (V&V) em Robótica 

A Verificação e Validação representam processos sistemáticos essenciais para garantir que sistemas robóticos atendam aos requisitos especificados e funcionem conforme o esperado em seu ambiente operacional. Em robótica, a V&V envolve testes rigorosos de hardware e software para identificar falhas, limitações operacionais e garantir confiabilidade. 
Objetivos Específicos: 

1. Identificar e documentar a versão específica do robô NAO disponível. 

2. Desenvolver e executar um plano de testes sistemático baseado na documentação oficial. 

3. Gerar uma Matriz de Capacidades Operacionais completa do robô. 

### 4. Implementar e validar um protótipo funcional de assistente virtual para o laboratório. 
#### 4 MATERIAIS E MÉTODOS 

#### 4.1 Materiais e Equipamentos 

Robô NAO (modelo e versão a serem identificados) 

Rede Wi-Fi institucional para comunicação 

Computador com Software da Fabricante (Choregraphe) 

Ambiente Python para desenvolvimento 

Documentação oficial do NAO (Aldebaran Documentation) 

#### 4.2 Fase 1: Metodologia de Identificação e Verificação 

#### 4.2.1 Identificação da Versão do NAO 

A identificação da versão específica do robô NAO será realizada seguindo protocolos estabelecidos pela documentação oficial, que incluem: verificação física de identificações no hardware, acesso à API do robô para utilização de ferramentas de diagnóstico integradas à plataforma NAOqi. 

#### 4.2.2 Matriz de Capacidades Operacionais 

Cada componente será classificado conforme seu estado operacional, avaliando em três níveis: 0 (inoperante), 1 (parcialmente funcional) e 2 (totalmente funcional), com documentação detalhada de desempenho. 

Será desenvolvida uma tabela com a Matriz abrangente para avaliação sistemática de cada subsistema do NAO, organizada nas seguintes categorias: 

#### 4.2.3 Matriz de Capacidades Operacionais em Camadas 

#### CAMADA 1: TESTES UNITÁRIOS (BASE) 

##### 1.1 TESTES DE SENSORES BÁSICOS 

Bateria - Nível de Carga (Prioridade Máxima) 

##### 1.2 TESTES DE JUNTAS UNITÁRIAS 

Cabeça - HeadYaw (Rotação Horizontal) 

Cabeça - HeadPitch (Inclinação Vertical) 

Ombros - LShoulderPitch e RShoulderPitch 

Joelhos - LKneePitch e RKneePitch 

Cotovelos - LElbowYaw e RElbowYaw 

Cotovelos - LElbowRoll e RElbowRoll 

Quadris - LHipPitch e RHipPitch 

Quadris - LHipRoll e RHipRoll 

Punhos - LWristYaw e RWristYaw 

Mãos - LHand e RHand 

Tornozelos - LAnklePitch e RAnklePitch 

Tornozelos - LAnkleRoll e RAnkleRoll 

#### CAMADA 2: TESTES DE INTEGRAÇÃO 

##### 2.1 INTEGRAÇÃO MEMBRO-COMPLETO 

Braço Esquerdo Completo (Ombro, Cotovelo, Punho e Mão) 

Braço Direito Completo (Ombro, Cotovelo, Punho e Mão) 

Perna Esquerda Completa (Quadril, Joelho, Tornozelo) 

Perna Direita Completa (Quadril, Joelho, Tornozelo) 

##### 2.2 INTEGRAÇÃO SENSOR-ATUADOR 

Sistema Visão + Movimento da Cabeça 

Sistema Equilíbrio + Sensores dos Pés 

Sistema Detecção de Obstáculos + Navegação 

CAMADA 3: TESTES DE SISTEMA 

##### 3.1 SUBSISTEMAS COMPLEXOS 

Sistema de Locomoção Completo 

Sistema de Manipulação de Objetos 

Sistema de Percepção Ambiental 

##### 3.2 COMPORTAMENTOS COMPLEXOS 

Postura em Pé 

Postura Sentado 

Postura Deitado 

Andar em Linha Reta (2 metros) 

Curva de 90 Graus 

Pegar Objeto do Chão 

Reação ao Toque na Cabeça 

Reação a Obstáculo Repentino 

#### CAMADA 4: TESTES DE ACEITAÇÃO 

##### 4.1 CENÁRIOS DE USO REAL 

Demonstração Básica de 5 Minutos 

Tarefa de Limpar Mesa 

Tarefa de Entregar Objeto 

Operação Contínua por 30 Minutos 

Múltiplas Tarefas Simultâneas 
