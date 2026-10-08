# Hibbes — Biblioteca

Librería de aprendizaje de League of Legends que construimos entre amigos: fundamentos, cada rol y cada campeón, con guías hechas de vídeos (enlaces) y notas. Se ve y se edita desde la sección **Biblioteca** de [Hibbes](https://github.com/dandmarspa-art/hibbes-releases/releases/latest).

Aquí no hay vídeos alojados: solo enlaces. Los de YouTube se reproducen dentro de Hibbes; los de Twitch, Vimeo u otras webs se abren en el navegador.

## Cómo contribuir

1. Pide al dueño del repo que te añada como colaborador y acepta la invitación.
2. En Hibbes: **Ajustes → Biblioteca → Crear token en GitHub** (token clásico, solo el permiso `public_repo`, con caducidad) y pégalo en **Conectar**.
3. En la Biblioteca pulsa **✎ Editar** para crear secciones, subsecciones, guías y lecciones.

Cada cambio hecho desde la app es un commit con tu usuario, así que todo queda en el historial y se puede deshacer.

## El archivo

Todo está en [`library.json`](library.json). Se puede editar a mano aquí en GitHub, pero es más fácil desde la app (valida el formato y evita pisar cambios de otros). Si el archivo queda inválido, Hibbes sigue mostrando su última copia buena hasta que se arregle.

- `sections`: carpetas (`parentId` = sección padre, `null` = nivel superior), con `icon` (un emoji).
- `guides`: cursos dentro de una sección (`sectionId`), con `difficulty` (`beginner`, `intermediate`, `advanced` o `null`), `champions` (ids de Data Dragon, p. ej. `MonkeyKing`) y `tags`.
- `lessons` (dentro de cada guía, en orden): `url` (solo `https://`, o `null` para una lección escrita) y `notes`. En las notas, los tiempos como `4:35` se pueden pulsar para saltar a ese momento del vídeo.

Hibbes no está respaldado por Riot Games y no refleja las opiniones de Riot Games ni de nadie involucrado oficialmente en la producción o gestión de las propiedades de Riot Games. League of Legends es una marca de Riot Games, Inc. Los vídeos enlazados pertenecen a sus autores.
