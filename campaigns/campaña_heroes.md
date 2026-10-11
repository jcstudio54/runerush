# Campaña de notificación — lanzamiento de los Héroes (0.4.3)

**Cuándo:** cuando la 0.4.3 pase la revisión de Google y esté publicada (testers primero).

## Imagen (1024 × 512, menos de 1 MB)
- `heroes_launch_es.jpg` — con título "¡Llegaron los Héroes!" (testers / español)
- `heroes_launch_en.jpg` / `heroes_launch_pt.jpg` — para producción
- `heroes_launch_notext.jpg` — sin texto (por si se prefiere)
Subirla a GitHub Pages (repositorio de jcstudio54.github.io), por ejemplo a
`runerush/img/heroes_launch_es.jpg`, y en Firebase pegar la URL directa:
`https://jcstudio54.github.io/runerush/img/heroes_launch_es.jpg` (abrirla antes en el navegador:
tiene que verse sólo la imagen).

## Texto (español)
- **Título:** ¡Llegaron los Héroes! ⚔️
- **Texto:** Aldric, Pyra y Sylva se unen a tu aventura: elige a tu héroe, carga su poder y libera
  su magia contra los Guardianes corrompidos. ¡Actualiza y juega!

(Inglés, para producción) **The Heroes Have Arrived! ⚔️** — Aldric, Pyra and Sylva join your
adventure: choose your hero, charge their power and unleash their magic against the corrupted Guardians.
Update and play!
(Portugués) **Os Heróis Chegaram! ⚔️** — Aldric, Pyra e Sylva se juntam à sua aventura: escolha
seu herói, carregue o poder e liberte a magia contra os Guardiões corrompidos. Atualize e jogue!

## Configuración en Firebase (Messaging → Nueva campaña → Notificaciones)
1. **Notificación:** título y texto de arriba; **Imagen:** la URL de GitHub Pages; nombre interno
   "Lanzamiento héroes 0.4.3".
2. **Orientación:** App `com.runerush.matchmagic` + Idiomas = español (las 4 variantes).
   (En producción: una campaña igual por idioma: inglés y portugués con su texto e imagen.)
3. **Programación:** "Ahora" (o un horario de tarde, 18-20 h, cuando más se juega).
4. **Eventos clave:** métrica objetivo `level_start`; etiqueta de Analytics `heroes_lanzamiento`.
5. **Opciones adicionales:** Canal `general`; Sonido habilitado; Vencimiento **3 días**.
6. Revisar → Publicar.

## Después
- En Messaging → la campaña: ver Enviados / Abiertos y cuántos jugaron un nivel después.
- En Analytics: evento `hero_power` y el parámetro `hero` de `level_start` muestran qué héroe eligen.
