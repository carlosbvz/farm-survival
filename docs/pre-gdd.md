# Documento de Concepto de Juego (Pre-GDD) — Survival (Prototype)

**Nombre del Proyecto:** Survival (Prototype)
**Versión:** 1.0.0
**Última Actualización:** Enero 31, 2026
**Preparado por:** Marcelo y Tio Calin

> **Enfoque del Prototipo:**  
> Este prototipo valida si la micro-gestión activa de plantas (cambiar de muro a atacante) es divertida y manejable bajo presión, o si resulta abrumadora. También valida el equilibrio entre la codicia económica (Día) y la dificultad de la horda (Noche).
>
> **Fuera de alcance:** Historia profunda, cinemáticas, multijugador, variedad masiva de plantas (solo las esenciales para probar la mecánica).

---

## 1. Resumen Ejecutivo

**Pitch en una Frase:**  
Un híbrido de *Tower Defense* y supervivencia donde gestionas una granja económica de día para sobrevivir a hordas de monstruos de noche mediante el comando activo de unidades botánicas.

**Pitch Elevator (30 segundos):**  
En *Survival (Prototype)*, el jugador debe equilibrar la codicia con la seguridad. Durante el día, el objetivo es expandir una red de plantas generadoras de recursos para financiar defensas. Al caer la noche, el juego se transforma en un desafío de resistencia donde insectos y jefes atacan tanto al jugador como a su fuente de ingresos. La tensión principal radica en decidir cuánto invertir en economía frente a cuánto invertir en protección, dentro de un ciclo constante de gestión, combate y escape.

---

## 2. Concepto Central

### 2.1 Descripción General del Juego
*Survival (Prototype)* es un juego de estrategia y supervivencia con mecánicas de *Tower Defense* activo. El jugador asume el rol de un protector de un jardín místico, gestionando una economía de plantas mientras despliega unidades de combate.

El juego se estructura en partidas finitas con ciclo día/noche. Entre partidas, el jugador progresa mediante un sistema de "Gacha" (paquetes misteriosos) para mejorar su arsenal.

#### Clasificación de Unidades (Plantas):
1. **Plantas Generadoras:** Unidades pasivas que producen moneda. Son el motor económico y objetivo principal enemigo.
2. **Plantas de Acción (Unidades Versátiles):** Unidades híbridas que el jugador alterna con interacción directa:
   * **Modo Defensivo (Muralla):** Se ancla al terreno con alta resistencia. Bloquea enemigos si su ataque es inferior a la defensa.
   * **Modo Ofensivo (Escolta/Asalto):** Se moviliza. Puede ser **Escolta** (protege al jugador) o **Unidad de Asalto** (caza enemigos en el mapa).

#### Meta-Progreso (Lobby):
Una tienda central donde se usan recursos de batalla para comprar **Paquetes Misteriosos**. Estos contienen semillas o mejoras con diferentes rarezas, permitiendo personalizar el mazo de defensa (*Deck Building*).

### 2.2 Género(s)
- **Principal:** Estrategia / Tower Defense Activo
- **Secundario:** Supervivencia / Gestión de Recursos / Roguelite (Meta-progresión)
- **Inspiraciones:** *Plants vs. Zombies* (Economía), *Vampire Survivors* (Hordas), *Kingdom: Two Crowns* (Gestión de codicia/defensa).

### 2.3 Público Objetivo
- **Jugador Principal:** Fans de estrategia que buscan una experiencia más mecánica y menos pasiva ("clicker").
- **Plataforma(s):** PC (Steam/Itch.io) y Móviles (el menú radial es ideal para pantallas táctiles).

---

## 3. Bucle Principal de Juego

### 3.1 Bucle Primario (Core Loop)
1. **Día (Gestión):** Plantar generadoras y organizar defensa estática.
2. **Noche (Acción):** Hordas atacan. El jugador corre por el mapa cambiando modos de plantas (Defensa $\leftrightarrow$ Ataque) según la amenaza.
3. **Resolución:** Sobrevivir al tiempo o matar al Jefe.
4. **Recompensa:** Obtención de moneda y semillas.
5. **Lobby:** Compra de paquetes misteriosos para mejorar el mazo.

### 3.2 Estructura de Progresión
* **Early Game:** Aprender a cambiar modos y proteger la primera generadora.
* **Mid Game:** Enemigos con habilidades (voladores, excavadores) que obligan a usar el modo "Asalto".
* **End Game:** Optimización de mazos para enfrentar Jefes masivos con múltiples fases.

### 3.3 El "Gancho" (The Hook)
Romper la pasividad del *Tower Defense*. Tus torres tienen "patas" y tú decides cuándo usarlas. La tensión de desmantelar tu propia muralla para salir a cazar al jefe.

---

## 4. Mecánicas Principales

### 4.1 Mecánicas Clave
1. **Gestión Táctica (Menú Radial):**
   * Click en planta $\rightarrow$ Menú Radial.
   * Opciones: Mejorar, Vender, Modo Muralla, Modo Escolta, Modo Asalto.
   * **Propósito:** Control total y adaptación en tiempo real.
2. **Economía de Meta-Progreso (Gacha):**
   * Tienda de Combate (Defensas) y Tienda Económica (Generadoras).
   * Compra de "Paquetes Misteriosos" con oro acumulado.
3. **Sistema de Incursión (IA):**
   * Enemigos salen de cuevas. Priorizan: Jugador (daño) o Generadoras (economía).
   * El jugador debe interceptar físicamente o bloquear rutas.

### 4.2 Mecánicas de los Enemigos
* **Escalado:** HP y Daño aumentan con el tiempo.
* **Variantes:** Rápidos (Zergling), Tanques (Lentos, alto HP), Destructores (Ignoran jugador, van directo a las plantas).

### 4.3 Ajuste y Sensación (Game Feel)
* **Feedback de Transformación:** Transición visual clara (ej. la planta "desenraíza" sus patas con un sonido de tierra rompiéndose) al cambiar a modo Asalto.
* **Impacto de Muralla:** Cuando un enemigo golpea una muralla, debe haber un *screen shake* leve o un efecto de partícula de "bloqueo" para sentir la resistencia.
* **Claridad del Menú Radial:** Al abrir el menú, el tiempo se ralentiza un 50% (efecto *slow-motion*) para dar al jugador un respiro táctico sin detener la acción.

---

## 5. Mundo y Narrativa

### 5.1 Ambientación
* **Estilo Visual:** "Jardín Sintético" o "Bio-Punk Luminoso". Una mezcla de naturaleza orgánica con energía mágica/tecnológica brillante.
* **Perspectiva:** Top-Down (Vista de pájaro) o Isométrica limpia para facilitar la lectura del mapa.
* **Tono:** Vibrante pero peligroso. Colores saturados de día, contrastes altos y sombras profundas de noche.

### 5.2 Narrativa
* **Premisa:** Eres el último "Jardinero" en un mundo consumido por la Plaga (insectos mutantes).
* **Conflicto Principal:** Purificar la tierra planta por planta. Las cuevas son heridas en el mundo que debes sellar sobreviviendo a lo que sale de ellas.

---

## 6. Características Clave y Diferenciación

### 6.1 Propuesta de Valor Única (USP)
* **Micro-Gestión vs Macro-Estrategia:** A diferencia de otros TD donde solo "construyes", aquí también "comandas".
* **Riesgo/Recompensa Dinámico:** Convertir tu mejor defensa (Muro) en tu mejor ataque (Asalto) deja tu base vulnerable. Esa decisión segundo a segundo es única.

---

## 7. Experiencia del Jugador

### 7.1 Emociones Buscadas
* **Día:** Ambición y Calma. ("¿Puedo permitirme plantar otra generadora o debo guardar para una defensa?").
* **Noche:** Pánico Controlado y Heroísmo. ("¡La muralla va a caer, necesito transformarla en atacante y pelear cuerpo a cuerpo!").

### 7.2 Dificultad y Accesibilidad
* **Curva:** Empieza lento (fácil entender muro vs. atacante). Escala rápido introduciendo enemigos que requieren cambios de modo específicos.
* **Accesibilidad:** El menú radial debe ser grande y claro. Uso de códigos de color (Verde = Economía, Azul = Defensa, Rojo = Ataque).

---

## 8. Dirección Artística y Sonora

### 8.1 Estilo Visual
* **Personajes (Plantas):** Diseños tiernos pero con "dientes". Que se vean robustas en modo muralla y ágiles en modo asalto.
* **UI (Interfaz):** Minimalista. Lo más importante es ver el campo de batalla. Indicadores de salud sobre las plantas.

### 8.2 Dirección de Audio
* **Música:**
  * **Día:** Acústica, relajante, sonidos de viento y hojas (*Lo-Fi beats*).
  * **Noche:** Sintetizadores oscuros, ritmo acelerado, percusión tribal.
* **SFX:** Crujidos de madera, disparos de semillas "secos" y satisfactorios, chillidos de insectos al morir.

---

## 9. Alcance y Escala

### 9.1 Alcance del Prototipo / v0.x
* **Objetivo:** Validar el "Game Feel" del cambio de modos y el Menú Radial.
* **Contenido Incluido:**
  * 1 Mapa (Arena simple con 2 cuevas).
  * 1 Personaje Jugador.
  * 3 Tipos de Planta: Generadora (Girasol), Muralla/Tanque (Nuez), Atacante Rápido (Guisante).
  * 2 Enemigos: Básico y Rápido.
* **Timeline:** 4 a 6 Semanas.

### 9.2 Post-Prototipo / Ideas Futuras
* Evolución de plantas (Fusionar dos plantas para crear una híbrida).
* Ciclos climáticos que afecten la producción.
* Modo cooperativo.

---

## 10. Métricas de Éxito
* **Validación de Diseño:** ¿Los jugadores usan los 3 modos de la planta? (Si solo usan "Muralla", el diseño falló).
* **Claridad:** ¿Entienden los jugadores intuitivamente cómo abrir el menú radial?
* **Técnico:** Mantener 60 FPS con 50+ enemigos en pantalla.

---

## 11. Preguntas Abiertas y Próximos Pasos

### 11.1 Preguntas Abiertas
* [ ] ¿Es divertido perseguir enemigos manualmente o debería ser automático dentro de un rango?
* [ ] ¿El menú radial interrumpe demasiado el flujo de combate frenético? (Probar la ralentización del tiempo).
* [ ] ¿Cómo evitamos que el jugador se quede sin recursos y sea imposible recuperarse (*Soft-lock*)?

### 11.2 Próximos Pasos
* [ ] **Crear Repositorio:** Configurar proyecto en Unity/Godot/Unreal.
* [ ] **Greybox:** Implementar movimiento del jugador y sistema de spawning básico.
* [ ] **Prototipar Menú Radial:** Crear la UI básica para seleccionar modos y probar la sensación de control.

---

**Fin del Documento**
