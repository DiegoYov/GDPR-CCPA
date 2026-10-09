# 📖 Guía del Docente y Notas de Exposición (Speaker Notes)
## Normativa, Ética y Privacidad de Datos en la Inteligencia Artificial (Masterclass 5 Horas)

Esta guía contiene el guion paso a paso, explicaciones técnicas a fondo, noticias reales, casos históricos y preguntas detonantes para cada una de las diapositivas de la presentación interactiva [`presentacion_etica_ia.html`](./presentacion_etica_ia.html).

---

## 🕒 Módulo 1: Marco Legal y Gobernanza (Hora 1 - Teórica)

---

### 📌 Slide 01: Portada — Ética, Datos y Normativa en la Era de la IA
* **Propósito:** Captar la atención inmediata del grupo y delimitar la tesis central: *La IA no opera en un vacío legal ni ético*.
* **Qué decir:**
  > "Bienvenidos a esta sesión sobre Normativa, Ética y Privacidad de Datos en la Inteligencia Artificial. Hoy no solo vamos a discutir teoría jurídica; vamos a entender la arquitectura técnica y legal detrás de los modelos modernos. Cuando un sistema de Machine Learning aprende de millones de interacciones, surge la pregunta crítica: ¿quién protege lo que la máquina sabe de ti y qué responsabilidades asumen quienes diseñan y consumen estos algoritmos?"
* **Acción en el HTML:** Mostrar la portada y los badges temáticos.

---

### 📌 Slide 02: Estructura de la Sesión (5 Horas)
* **Propósito:** Brindar el mapa de ruta pedagógico (1 hora teórica + 4 horas de taller práctico dividido en 4 bloques).
* **Qué decir:**
  > "Nuestra jornada de 5 horas se divide en dos grandes fases. La primera hora será nuestra base teórica: GDPR, CCPA, Ley 1581 de Colombia y el EU AI Act. Las siguientes 4 horas serán 100% prácticas:
  > * **Bloque A:** Flujos transfronterizos y consumo seguro de APIs cloud (OpenAI, AWS, Azure).
  > * **Bloque B:** Técnicas de preservación de privacidad (PETs), ataques de inferencia y sanitización con Microsoft Presidio.
  > * **Bloque C:** Auditoría algorítmica, métricas de equidad (Fairness), explicabilidad (XAI) y marcos NIST.
  > * **Bloque D:** Taller grupal con auditoría de una Ficha Técnica simulada de triaje médico."

---

### 📌 Slide 03: ¿Qué es un dato personal y qué es tratamiento?
* **Propósito:** Unificar conceptos técnicos y legales fundamentales según la doctrina internacional y colombiana.
* **Qué decir:**
  > "Antes de hablar de algoritmos, definamos la materia prima: el **dato personal**. No es solo tu nombre o tu cédula. Es cualquier dato que permita identificarte de forma directa o indirecta (por ejemplo, una dirección IP combinada con coordenadas GPS o un vector de embeddings).
  > El **tratamiento** abarca TODO el ciclo de vida: desde que un script raspa una web o captura un formulario, pasando por el almacenamiento en bases vectoriales, hasta el prompting y la supresión final.
  > Especial atención a los **datos sensibles**: salud, biometría, ideología, orientación sexual. Su tratamiento está prohibido por defecto salvo excepciones muy estrictas."
* **Pregunta detonante:** *"¿Consideran que la huella de voz o el patrón de tecleo de una persona es un dato personal o un dato sensible?"*

---

### 📌 Slide 04: Principio de Minimización (Datos Necesarios vs. Excesivos)
* **Propósito:** Enseñar el principio de *Privacy by Design* aplicado a productos digitales reales.
* **Qué decir:**
  > "El principio de minimización (Art. 5.1.c GDPR) dice que solo debemos recolectar los datos **estrictamente necesarios** para la finalidad del servicio. Históricamente, las empresas capturaban todo 'por si acaso'. En la era de la IA, capturar datos de más es un pasivo legal y un riesgo de fuga."
* **Acción interactiva:** Hacer clic en cada una de las 6 pestañas (*Domicilios, Banca, Salud, Red Social, Educación, Chatbot GenAI*) y debatir por qué los datos marcados en rojo son ilegítimos o desproporcionados.
* **Punto clave:** En el Chatbot GenAI, resaltar que retener conversaciones indefinidamente o re-entrenar modelos públicos con prompts de clientes viola la minimización y el secreto profesional.

---

### 📌 Slide 05: Pregunta de Transición y Debate
* **Propósito:** Pausa pedagógica detonante para conectar la arquitectura de apps con el marco legal.
* **Pregunta central:**
  > **"¿Quién regula qué datos podemos o no podemos recolectar?"**
* **Qué decir:**
  > "Si una startup o una multinacional crea un modelo de IA que escucha micrófonos o procesa historiales médicos... ¿quién fija los límites? No es la tecnología la que se autorregula; existen tres capas regulatorias: tratados internacionales como el GDPR, leyes estatales comerciales como la CCPA y normativas locales como la Ley 1581 de Colombia."

---

### 📌 Slide 06: Los Dos Gigantes Regulatorios — GDPR & CCPA (Hero)
* **Propósito:** Impacto visual monumental para presentar las dos fuerzas que dominan el panorama de privacidad mundial.
* **Qué decir:**
  > "La respuesta a la pregunta anterior tiene dos grandes protagonistas. A nivel global, el mundo digital no está regulado por cientos de leyes inconexas, sino por dos gigantes normativos que dictan cómo se construye software e Inteligencia Artificial en todo el planeta: **GDPR** desde la Unión Europea y **CCPA** desde California, Estados Unidos."

---

### 📌 Slide 07: ¿Qué son exactamente GDPR y CCPA?
* **Propósito:** Brindar la definición formal, el significado explícito de las siglas y la diferencia de filosofía jurídica.
* **Qué decir:**
  > "Desglosemos exactamente qué significan estas siglas y qué hace cada una:
  > * **GDPR (*General Data Protection Regulation*):** Es el Reglamento Europeo 2016/679, vigente desde mayo de 2018. Aplica a **cualquier empresa del planeta** que trate datos de residentes en la UE. Su filosofía: la privacidad es un **derecho humano fundamental e inalienable del ciudadano**.
  > * **CCPA (*California Consumer Privacy Act*):** Es la ley de California (donde operan OpenAI, Meta, Google, Apple), vigente desde enero de 2020. Aplica a empresas comerciales. Su filosofía: proteger al **consumidor frente al mercado y la venta no consentida de su información**.
  > En resumen: el GDPR protege al **ciudadano**; la CCPA protege al **consumidor**."

---

### 📌 Slide 08: GDPR (Europa) — Principios y Derechos
* **Propósito:** Desglosar los principios técnicos y legales del Reglamento General de Protección de Datos.
* **Qué decir:**
  > "El GDPR cambió las reglas del juego bajo cuatro pilares técnicos:
  > 1. **Minimización (Art. 5.1.c):** Prohibido recolectar datos 'por si acaso'. Solo lo estrictamente necesario.
  > 2. **Opt-in explícito (Art. 7):** Sin un 'SÍ' activo, libre e informado, cualquier tratamiento es nulo.
  > 3. **Derecho al Olvido (Art. 17):** Obligación de suprimir y desindexar datos al revocarse el consentimiento.
  > 4. **Derechos ARCO/POLSO:** Acceso, Rectificación (clave frente a alucinaciones de IA), Cancelación, Oposición, Portabilidad y Limitación.
  > 5. **Sanciones disuasorias:** Hasta el **4% de la facturación global anual** de la corporación o **€20 Millones**."

---

### 📌 Slide 09: GDPR en Titulares y Casos Históricos
* **Propósito:** Aterrizar el GDPR en noticias de impacto mundial que demuestran su poder real frente a Big Tech e IA.
* **Historias y noticias para explicar en detalle:**
  1. **El Gran Detonante: Cambridge Analytica (2018):**
     * *Historia:* En 2014, Aleksandr Kogan creó la app "thisisyourdigitallife" en Facebook. 270.000 personas la descargaron, pero la API permitía extraer datos de toda la red de amigos.
     * *Resultado:* Cosecharon los datos de **87 millones de personas** sin autorización. Cambridge Analytica usó el modelo psicológico OCEAN para perfilar votantes y lanzar *Dark Posts* micro-segmentados en las elecciones de EE. UU. (Trump 2016) y el Brexit.
     * *Impacto:* Aceleró la entrada en vigor del GDPR en mayo de 2018 con respaldo social unánime.
  2. **La Mayor Multa de la Historia: Meta (€1.200 Millones - 2023):**
     * Sanción récord de la autoridad irlandesa (DPC) a Meta por transferir datos de europeos a servidores en EE. UU. sin salvaguardas frente a la vigilancia estatal (*Schrems II*).
  3. **El Bloqueo a OpenAI en Italia (Marzo 2023):**
     * El *Garante Privacy* bloqueó ChatGPT en Italia por entrenar con datos masivos de internet sin base jurídica, falta de filtros de edad y alucinaciones falsas sobre personas reales (violación del Derecho de Rectificación). OpenAI tuvo que añadir formularios de exclusión y borrado de PII.
* **💡 Dilema de la IA:** ¿Cómo garantizas el "Derecho al Olvido" si un dato personal ya fue absorbido por los pesos neuronales? *Técnicamente, no se puede 'des-entrenar' un parámetro aislado sin re-entrenar el modelo.*

---

### 📌 Slide 10: CCPA / CPRA (California) — "No vendan mi información"
* **Propósito:** Analizar a fondo el modelo de California y el mecanismo de Opt-out.
* **Qué decir:**
  > "La CCPA opera bajo el modelo **Opt-out**: el tratamiento comercial está permitido hasta que el usuario dice **'Do Not Sell or Share My Personal Information'**. Si el usuario lo activa, la empresa no puede ceder sus datos a brokers de datos ni usarlos para entrenar modelos de IA de terceros, ni cobrarle más por ejercer su derecho."
* **Acción interactiva:** Hacer clic en el botón *"🚫 Do Not Sell My Personal Information"*.

---

### 📌 Slide 11: CCPA en Titulares y Casos Históricos
* **Propósito:** Mostrar sanciones reales de la Fiscalía de California y demandas colectivas contra gigantes de IA.
* **Historias y noticias para explicar en detalle:**
  1. **El Caso Histórico de Sephora ($1.2 Millones - 2022):**
     * *Hechos:* Sephora instaló trackers de analítica de terceros en su web que recolectaban datos de navegación y compras. Sephora no consideraba esto una 'venta', pero la Fiscalía de California dictaminó que entregar datos a redes publicitarias a cambio de servicios analíticos califica legalmente como **VENTA**. Además, no procesaba las señales del *Global Privacy Control (GPC)*.
     * *Lección:* Compartir telemetría de usuarios con APIs externas sin botón de Opt-out es ilegal en California.
  2. **Rastreo Engañoso de Google ($93 Millones - 2023):**
     * *Hechos:* Google informaba a los usuarios que desactivar el 'Historial de ubicaciones' detenía el rastreo. Sin embargo, seguía capturando coordenadas GPS a través de la actividad web y de aplicaciones (*Web & App Activity*). California demandó y multó a Google por prácticas comerciales engañosas.
  3. **Demandas Colectivas contra OpenAI y Meta en California (2023–2024):**
     * *Hechos:* Grupos de autores (como Sarah Silverman y Paul Tremblay) demandaron a OpenAI y Meta en los tribunales federales de San Francisco por raspar internet y absorber sus datos e historias personales para entrenar ChatGPT y LLaMA sin darles una opción de *Opt-out* ni compensación.
* **💡 La Regla de Oro en California para IA:** Si utilizas datos capturados de tus usuarios para calibrar o entrenar un modelo comercial de un tercero (o cederlos a OpenAI/Google), legalmente estás realizando una **VENTA DE DATOS**. Requiere obligatoriamente el enlace *Do Not Sell or Share*.

---

### 📌 Slide 12: El "Efecto Bruselas" (Globalización de la Norma)
* **Propósito:** Explicar cómo la UE y EE. UU. dictan las reglas del software en todo el mundo.
* **Qué decir:**
  > "El 'Efecto Bruselas' explica que las multinacionales prefieren adaptar su producto global a la ley más exigente (GDPR/CCPA) antes que mantener software fragmentado por países. Por eso, una app desarrollada en Colombia hereda estas obligaciones si usa infraestructura o SDKs globales."

---

### 📌 Slide 13: Pregunta — ¿Y qué normas locales existen?
* **Propósito:** Abrir la reflexión sobre por qué la ley internacional no basta y por qué la cultura local y la soberanía exigen leyes propias.
* **Qué decir:**
  > "Si el GDPR y la CCPA ya existen… ¿por qué cada país necesita su propia ley?
  > 1. **Cerrar vacíos legales:** Si no tenemos ley local, las multinacionales tratarán a nuestros países como 'paraísos de datos', experimentando sin consecuencias.
  > 2. **La cultura de la evasión e informalidad:** Frente a la mentalidad de 'hecha la ley, hecha la trampa', se requieren inspectores y autoridades con poder sancionatorio ejecutable en nuestro territorio.
  > 3. **Soberanía jurídica:** Un ciudadano común en Bogotá o Buenos Aires no tiene los recursos para demandar a OpenAI en California o Bruselas; necesita a su autoridad local para defenderlo."

---

### 📌 Slide 14: América Latina — Marco Regional y Escándalos de IA
* **Propósito:** Conectar el panorama de LatAm con el mayor escándalo biométrico reciente de la región.
* **Puntos clave y noticias para exponer:**
  * **LGPD de Brasil:** Es el GDPR de América Latina. En julio de 2024, la autoridad brasileña (ANPD) le puso un freno histórico a Meta, prohibiéndole entrenar sus modelos de IA con posts y fotos de usuarios de Instagram/Facebook sin consentimiento explícito.
  * **Argentina, Chile y México:** Marcos con tradición de protección de datos (Argentina fue el primer país de la región declarado adecuado por la UE; Chile actualizó su ley al estándar europeo en 2024).
  * **👁️ El Gran Escándalo Regional: Worldcoin / Tools for Humanity (2023–2024):**
    * *Qué ocurrió:* La empresa cofundada por Sam Altman instaló esferas metálicas (*Orbs*) en centros comerciales y plazas de Argentina, Colombia, Chile y Brasil, ofreciendo criptomonedas (tokens WLD) a cambio de **escanear el iris del ojo**.
    * *El dilema ético y legal:* Millones de personas en situación de vulnerabilidad económica entregaron su dato biométrico más sensible e irreemplazable (no puedes cambiar tu iris como cambias una contraseña) sin entender qué harían con él, sin validación estricta de edad de menores y sin servidores locales.
    * *Consecuencias:* Multas récord de la AAIP en Argentina, investigaciones activas de la SIC en Colombia y suspensiones en varios países.

---

### 📌 Slide 15: Marco Normativo en Colombia
* **Propósito:** Aterrizar en la legislación colombiana y la responsabilidad local.
* **Puntos clave:**
  * **Ley 1581 de 2012:** Autorización previa, expresa e informada.
  * **Superintendencia de Industria y Comercio (SIC):** Multas de hasta 2.000 SMLMV e investigaciones de oficio (como en el caso Worldcoin).
  * **MinCiencias:** "Ruta de adopción ética y sostenible de IA".
  * **CONPES 4144:** Política Nacional de IA.
* **Advertencia:** Enviar datos de colombianos a servidores en EE. UU. sin cumplir el Art. 26 de la Ley 1581 es una transferencia internacional no autorizada.

---

### 📌 Slide 16: Universalidad: Del Hardware (USB-C) a los Algoritmos (AI Act)
* **Propósito:** Consolidar con una analogía física tangible: *la ley transforma la tecnología*.
* **Qué decir:**
  > "Así como la UE obligó a Apple a adoptar USB-C en el iPhone 15 para todo el mundo, el **EU AI Act de 2024** establece los estándares globales de seguridad y transparencia algorítmica."

---

## 🕒 Módulo 2: Flujos Transfronterizos y Arquitectura Cloud (Hora 2 - Taller Bloque A)

---

### 📌 Slide 17: El Viaje del Dato: APIs Cloud de Terceros
* **Propósito:** Comprender la implicación jurídica de invocar endpoints como `openai.ChatCompletion.create()`.
* **Qué decir:**
  > "Cuando una app en Colombia envía un prompt con datos personales a la API de OpenAI en EE. UU., ocurre una **Transferencia Internacional de Datos**. Se requiere DPA (Data Processing Addendum) y Cláusulas Contractuales Tipo (SCCs)."

---

### 📌 Slide 18: Políticas de Datos de APIs: Consumer vs. Enterprise
* **Propósito:** Marcar la diferencia crítica entre cuentas públicas gratuitas y APIs comerciales.
* **Qué decir:**
  > "* **Consumer (gratuito):** Datos retenidos y usados para re-entrenar modelos.
  > * **Enterprise / API Comercial:** Garantías de *No-Training* y *Zero Data Retention (ZDR)*."

---

### 📌 Slide 14: Patrón de Arquitectura: Privacy Gateway
* **Propósito:** Enseñar a los estudiantes el patrón técnico de intermediación segura para proteger datos antes de tocar la nube.
* **Flujo del diagrama:**
  1. Frontend captura el input del usuario.
  2. **Gateway On-Premise:** Detecta PII, reemplaza los datos con tokens sintéticos y guarda la relación cifrada en una bóveda local (*Vault*).
  3. **Cloud API:** El LLM en la nube recibe el texto completamente anonimizado y razona sobre las variables.
  4. **Gateway Inverso:** Reemplaza los tokens de vuelta solo para mostrarle la respuesta final al usuario autenticado.

---

## 🕒 Módulo 3: Técnicas de Privacidad y PETs (Hora 3 - Taller Bloque B)

---

### 📌 Slide 15: La Tríada Técnica: Anonimización vs. Seudonimización vs. Encriptación
* **Propósito:** Clarificar la diferencia técnica y legal entre estos tres conceptos que comúnmente se confunden.
* **Explicación técnica:**
  * **Anonimización:** Proceso **irreversible**. Rompe todo vínculo con el titular. Legalmente *deja de ser dato personal*.
  * **Seudonimización:** Proceso **reversible mediante una clave o tabla de correspondencia**. Legalmente *SIGUE SIENDO dato personal* (Art. 4.5 GDPR).
  * **Encriptación:** Transformación algorítmica matemática (AES-256 en reposo, TLS 1.3 en tránsito, Cifrado Homomórfico en cómputo).

---

### 📌 Slide 16: PETs Avanzadas: K-Anonimato y Privacidad Diferencial (ε)
* **Propósito:** Introducir conceptos matemáticos de privacidad aplicados a Data Science y Machine Learning.
* **Conceptos clave:**
  * **K-Anonimato:** En una tabla, cada individuo debe compartir sus cuasi-identificadores (ej. edad agrupada '30-40', código postal '110xxx') con al menos $k-1$ personas.
  * **Privacidad Diferencial ($\epsilon$):** Inyección controlada de ruido matemático (Laplace o Gaussiano) para que sea imposible deducir si una persona específica estaba o no en el conjunto de datos de entrenamiento ($DP-SGD$).

---

### 📌 Slide 17: Vulnerabilidades y Ataques de Inferencia en LLMs
* **Propósito:** Sensibilizar sobre los vectores de ataque dirigidos a modelos de lenguaje.
* **Ataques a explicar:**
  1. **Membership Inference Attack:** Un atacante envía preguntas específicas para medir la probabilidad de salida y averiguar si un paciente con cáncer fue parte del dataset.
  2. **Model Inversion / Reconstruction:** El atacante logra reconstruir fragmentos exactos de texto confidencial memorizados por el modelo.
  3. **Prompt Injection / Data Extraction:** Instrucciones adversarias que fuerzan al modelo a volcar variables del sistema o números de tarjetas de crédito.

---

### 📌 Slide 18: Simulador Interactivo: Microsoft Presidio y Regex
* **Propósito:** Práctica en vivo en la presentación para ver cómo opera un pipeline de sanitización NLP.
* **Acción interactiva:**
  * Probar los botones *"Caso Médico"*, *"Caso Financiero"* y *"Caso Estudiante"*.
  * Presionar **"⚡ Ejecutar Presidio Anonymizer"**.
  * Mostrar cómo se detectan y enmascaran nombres, cédulas colombianas, teléfonos, emails y diagnósticos sensibles, mostrando estadísticas de entidades en tiempo real.

---

### 📌 Slide 19: Código Python de Referencia (Presidio Pipeline)
* **Propósito:** Proveer el script real que los estudiantes pueden implementar en sus aplicaciones.
* **Qué destacar en el código:**
  * `AnalyzerEngine` y `AnonymizerEngine` de Presidio.
  * Creación de un `PatternRecognizer` con Regex para cédulas colombianas de 7 a 10 dígitos.
  * Uso de `OperatorConfig` con máscara parcial (`******`) o reemplazo de entidad (`<PACIENTE>`).

---

## 🕒 Módulo 4: Auditoría, Fairness y Explicabilidad (XAI) (Hora 4 - Taller Bloque C)

---

### 📌 Slide 20: Evaluación de Equidad (Métricas de Fairness)
* **Propósito:** Mostrar las fórmulas matemáticas para auditar sesgos algorítmicos.
* **Métricas:**
  * **Disparate Impact (Regla del 80%):** Si la tasa de aprobación de un grupo minoritario dividida entre la del grupo mayoritario es $< 0.80$, existe discriminación estadística ilegal.
  * **Demographic Parity:** La probabilidad de predicción positiva debe ser idéntica entre géneros o etnias.
  * **Equalized Odds:** Las tasas de falsos positivos y verdaderos positivos deben ser homogéneas.
* **Librerías recomendadas:** `Fairlearn` (Microsoft) y `AIF360` (IBM).

---

### 📌 Slide 21: Explicabilidad Técnica (XAI): SHAP y LIME
* **Propósito:** Superar el problema de la "Caja Negra" algorítmica para cumplir con el Art. 22 del GDPR.
* **Herramientas:**
  * **SHAP (Valores Shapley):** Mide la contribución exacta de cada variable (edad, ingresos, historial) a la predicción final.
  * **LIME:** Genera un modelo interpretable local alrededor de una decisión específica (útil para explicar por qué se denegó un crédito o un triaje médico).

---

### 📌 Slide 22: Marcos de Riesgo: NIST AI RMF y Checklist Pre-Producción
* **Propósito:** Dotar al equipo de una metodología de evaluación antes de desplegar a producción.
* **Marco NIST AI RMF 1.0:** *Govern, Map, Measure, Manage*.
* **Acción interactiva:** Interactuar con el **Checklist Pre-Producción** en la diapositiva para ver cómo cambia dinámicamente el nivel de riesgo (*Alto Riesgo*, *Riesgo Medio*, *Conforme*).

---

### 📌 Slide 23: Red Teaming y Seguridad Ofensiva en LLMs
* **Propósito:** Enseñar cómo auditar la seguridad de un modelo mediante pruebas de penetración.
* **Conceptos:** *Prompt Injections directas e indirectas*, *Jailbreaks* y *Guardrails* (NeMo Guardrails de NVIDIA, Llama Guard de Meta).

---

## 🕒 Módulo 5: Caso de Estudio, Casos Reales y Taller (Hora 5 - Taller Bloque D)

---

### 📌 Slide 24: Propiedad Intelectual en GenAI
* **Propósito:** Analizar la autoría y el copyright en la era de los modelos generativos.
* **Puntos clave:**
  * **Sin autoría humana no hay copyright:** Jurisprudencia de la Oficina de Derechos de Autor de EE. UU.
  * **Litigios de entrenamiento:** Demandas de *The New York Times vs. OpenAI* y *Getty Images vs. Stability AI* por usar millones de artículos e imágenes protegidas sin licencia.

---

### 📌 Slide 25: Casos Reales: Cuando la IA Colisiona
* **Propósito:** Aprender de fallos sonados de la industria:
  1. **Mata vs. Avianca (2023):** Abogado presentó en la corte de Nueva York precedentes judiciales inventados por ChatGPT. Sanción judicial por negligencia.
  2. **Fuga de Código en Samsung (2023):** Ingenieros subieron código fuente confidencial y minutas de reuniones a ChatGPT, filtrando secretos industriales.
  3. **Clearview AI:** Scraping de 30.000 millones de imágenes de redes sociales para reconocimiento facial. Multas superiores a €50M en Europa por violar la biometría.

---

### 📌 Slide 26: Uso Ético en el Contexto Académico
* **Propósito:** Normas claras para docentes y estudiantes:
  * **Permitido:** Planeación didáctica, generación de casos sintéticos y rúbricas.
  * **Prohibido:** Subir notas, nombres reales o diagnósticos de alumnos a chatbots públicos.

---

### 📌 Slide 27: 🚀 TALLER CENTRAL: Auditoría de la Ficha Técnica "MediBot-Triaje AI"
* **Propósito:** Ejercicio grupal central de 30 a 45 minutos.
* **Ficha Técnica del caso a evaluar:**
  * *MediBot-Triaje AI (v1.2):* Asistente de urgencias médicas.
  * **Vulnerabilidades del caso:**
    1. Micrófonos en sala de espera grabando audio continuo (violación de consentimiento y datos sensibles).
    2. Envío de transcripciones crudas a la API de OpenAI en EE. UU. bajo cuenta estándar (fuga transfronteriza sin DPA/ZDR).
    3. Base de datos vectorial con biometría de voz y cédula sin anonimizar (incumplimiento de minimización).
    4. Algoritmo con sesgo que penaliza a mayores de 60 años de zonas rurales (violación de Fairness).
    5. Consentimiento por letrero en la pared (consentimiento oscuro e inválido).
* **Acción interactiva:** Iniciar el temporizador (15', 30' o 45') para coordinar el trabajo en salas o mesas.

---

### 📌 Slide 28: Ciclo de Vida, Responsabilidades y Tablero de Socialización
* **Propósito:** Cierre de la clase y puesta en común de las soluciones propuestas por los grupos.
* **Acción interactiva:** Invitar a los grupos a escribir sus hallazgos en el campo inferior y presionar Enter para crear notas adhesivas en el tablero en vivo.
* **Mensaje de cierre:**
  > *"La privacidad y la ética no son un añadido de última hora: son requerimientos arquitectónicos no negociables. Un buen desarrollador de IA no es solo quien maximiza la precisión del modelo, sino quien garantiza la seguridad y los derechos de las personas."*
