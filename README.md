# DevGen Credential

Generador de credenciales digitales para desarrolladores. Una tarjeta de perfil con identidad visual propia, diseñada para presentar información profesional de forma clara y atractiva.

## Sobre el proyecto

**DevGen Credential** es una aplicación web estática que renderiza una credencial de desarrollador al estilo tarjeta de identificación. Combina HTML semántico y CSS moderno para construir una interfaz limpia, con jerarquía visual definida y atención al detalle en espaciado, bordes y composición.

La tarjeta incluye:

- Encabezado con branding *DevGen*
- Imagen de perfil con degradado superpuesto
- Datos personales y profesionales (ciudad, email, tecnologías, hobby, GitHub)
- Frase destacada en el pie de la tarjeta

### Próximas mejoras

- [ ] Formulario interactivo para crear la credencial en tiempo real
- [ ] Vista previa dinámica al editar los campos
- [ ] Personalización de colores y estilo de la tarjeta

## Tecnologías

| Tecnología | Uso |
|------------|-----|
| HTML5 | Estructura semántica (`header`, `main`, `article`, `section`, `footer`) |
| CSS3 | Box Model, variables CSS, Flexbox, Grid, pseudo-elementos |
| Font Awesome | Iconografía |
| Google Fonts | Tipografía [Plus Jakarta Sans](https://fonts.google.com/specimen/Plus+Jakarta+Sans) |

## Fundamentos técnicos

El proyecto aplica conceptos del **CSS Box Model** de forma explícita:

| Concepto | Implementación |
|----------|----------------|
| `box-sizing: border-box` | Reset global para incluir padding y border en el ancho/alto total |
| `padding` | Espaciado interno en `.cardBody`, `.cardFooter` e `.infoContainer` |
| `border` | Bordes en iconos y footer de la tarjeta |
| `border-radius` | Esquinas redondeadas en tarjeta, iconos y footer |
| `width` / `height` | Dimensiones fijas de la tarjeta (400 × 620 px) |
| `box-shadow` | Sombra para dar profundidad a la credencial |

La paleta de colores se gestiona con variables CSS en `:root` (`--primary-color`, `--secondary-color`, `--tertiary-color`, etc.) para mantener consistencia visual.

## Estructura del proyecto

```
LAB_BoxModel/
├── index.html      # Estructura HTML de la credencial
├── style.css       # Estilos y layout de la tarjeta
└── README.md
```

## Cómo ejecutar

No requiere instalación ni dependencias. Abre `index.html` en tu navegador o usa una extensión de servidor local como Live Server.

## Autora

**Angélica García** — Fullstack Developer  
[GitHub @YessBlack](https://github.com/YessBlack)
