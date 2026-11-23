---
name: Кейс
colors:
  surface: '#fbf9f9'
  surface-dim: '#dbdad9'
  surface-bright: '#fbf9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f5f3f3'
  surface-container: '#efeded'
  surface-container-high: '#e9e8e7'
  surface-container-highest: '#e3e2e2'
  on-surface: '#1b1c1c'
  on-surface-variant: '#5a4138'
  inverse-surface: '#303031'
  inverse-on-surface: '#f2f0f0'
  outline: '#8f7066'
  outline-variant: '#e3bfb2'
  surface-tint: '#E65100'
  primary: '#E65100'
  on-primary: '#ffffff'
  primary-container: '#CC4800'
  on-primary-container: '#fffbff'
  inverse-primary: '#ffb59a'
  secondary: '#5f5e5e'
  on-secondary: '#ffffff'
  secondary-container: '#e2dfde'
  on-secondary-container: '#636262'
  tertiary: '#005ab7'
  on-tertiary: '#ffffff'
  tertiary-container: '#0072e4'
  on-tertiary-container: '#fefcff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdbcf'
  primary-fixed-dim: '#ffb59a'
  on-primary-fixed: '#380d00'
  on-primary-fixed-variant: '#802a00'
  secondary-fixed: '#e5e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1b1c1c'
  on-secondary-fixed-variant: '#474746'
  tertiary-fixed: '#d7e2ff'
  tertiary-fixed-dim: '#abc7ff'
  on-tertiary-fixed: '#001b3f'
  on-tertiary-fixed-variant: '#00458f'
  background: '#fbf9f9'
  on-background: '#1b1c1c'
  surface-variant: '#e3e2e2'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 26px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '600'
    lineHeight: 14px
    letterSpacing: 0.03em
  code-tabular:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '500'
    lineHeight: 18px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-desktop: 1.5rem
  margin: 1rem
  margin-desktop: 2rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 0.75rem
  space-lg: 1.25rem
  space-xl: 2rem
---

# Кейс — правила дизайна

## Стиль и основа
- **Три слова о стиле:** рабочий, светлый, чёткий
- **Главный цвет:** оранжевый `#E65100` (только кнопки, активное меню, акценты)
- **Примеры сайтов (идея и настроение, не копия):**
  1. <ВСТАВЬ ССЫЛКУ 1 (dribbble.com / behance.net)>
  2. <ВСТАВЬ ССЫЛКУ 2>
  3. <ВСТАВЬ ССЫЛКУ 3, по желанию>
- **Проект:** «Кейс» — информационная система учёта оборудования для выездных работ. Экраны: вход, каталог, карточка оборудования, мои выдачи, админ-панель оборудования.

## Не входит в MVP (не рисовать и не добавлять)
Фото оборудования, уведомления, отчёты и экспорт Excel/PDF, сканеры штрихкодов и RFID, оплата, чат, отзывы, самостоятельная регистрация. Сотрудник не видит, кто ещё брал оборудование (только срок возврата); историю по каждой единице видит только администратор.

## Brand & Style

This design system is engineered for internal hardware and equipment tracking environments. It embodies an industrial utilitarian minimalism inspired by tools like Linear, GitHub Enterprise, and dense technical consoles. The interface prioritizes structural clarity, instantaneous visual scanning, high contrast, and dense data legibility over decorative flourishes.

The target audience consists of hardware engineers, IT asset managers, lab technicians, and warehouse supervisors who handle individual equipment records, lifecycle audits, and check-in/check-out accountability. The user experience evokes absolute precision, stability, and operational efficiency without unnecessary cognitive overhead.

## Colors

The palette balances a focused, industrial orange primary tone against a stark, high-contrast monochrome foundation and functional semantic status colors.

### Key Palettes
- **Primary (`#E65100`)**: Deep vivid industrial orange used deliberately for primary interactive actions, high-priority state highlights, active navigation accents, and focal focus indicators.
- **Secondary (`#212121`)**: Deep carbon black used for structural text, primary labels, and secondary interactive borders.
- **Surface & Backgrounds**: Crisp canvas white (`#FFFFFF`) layered on neutral slate gray (`#F8F9FA` to `#F5F5F5`) for container segmentation. Hairline dividing borders use `#E0E0E0` (with `#D0D0D0` on interactive hover states).

### Semantic Equipment Status Badges
Status indicators must strictly adhere to the following badge definitions to eliminate cognitive latency:
- **Available / Доступно**: Background `#E8F5E9`, text `#1B5E20`.
- **In Use / Unassigned / Недоступно / На руках**: Background `#F5F5F5`, text `#616161`.
- **In Repair / Maintenance / В ремонте**: Background `#FFEBEE`, text `#C62828`.
- **Decommissioned / Списано**: Background `#EEEEEE`, text `#757575`.

## Typography

The design system standardizes on **Inter** across all UI layers. For serial numbers, inventory IDs, asset tags, and date columns, utilize `font-feature-settings: 'tnum' on, 'cv05' on` to ensure tabular alignment and clear character differentiation (e.g., distinguishing numeral `0` from letter `O`).

- Headings are concise, bold, and strictly restrained in scale to avoid displacing functional table views and forms.
- Data grids, metadata lists, and form controls rely on `body-md` (14px) and `label-md` (12px) for optimal information density without sacrificing legibility.
- Status badges and category chips use `label-sm` with slight tracking for swift recognition.

## Layout & Spacing

The layout employs a dense, structured fluid-grid layout bounded inside a maximum viewport container (`1440px`) or full-width data dashboard. 

- **Grid Model**: 12-column responsive layout with thin lines dividing the main views.
- **Rhythm**: Standard spacing aligns to an 8px grid baseline with 4px sub-increments (`0.25rem`, `0.5rem`, `0.75rem`, `1.25rem`, `2rem`) to maintain compact tool layouts.
- **Breakpoints**:
  - `Desktop (>= 1280px)`: top navigation bar (no sidebar), fluid data workspace, 24px column gutters.
  - `Tablet (768px - 1279px)`: Compact top navigation, 16px margins, tables convert to horizontally scrolling panes.
  - `Mobile (< 768px)`: Single-column flow with full-width action headers, sticky bottom actions, and 16px margins.

## Elevation & Depth

In alignment with industrial utilitarian minimalism, depth is achieved almost entirely through flat structural layering and crisp borders rather than soft, ambient shadows.

- **Layer 0 (Canvas)**: Background `#F8F9FA` or `#FFFFFF`.
- **Layer 1 (Cards, Panel Containers, Tables)**: Pure white `#FFFFFF` bounded by a solid 1px `#E0E0E0` border.
- **Layer 2 (Overlays, Flyouts, Slide-over Panels)**: Pure white surface with a 1px `#D0D0D0` border accompanied by an intentional, tight utility shadow: `0 4px 12px rgba(0, 0, 0, 0.08)`.
- **Active Focus**: `box-shadow: 0 0 0 2px #FFFFFF, 0 0 0 4px #E65100` for clear keyboard accessibility.

## Shapes

Geometry is intentionally firm and architectural:
- Base border radius is set to **`roundedness: 1`** (`0.25rem` / 4px).
- Inputs, action buttons, table cell containers, and status badges consistently adopt 4px corner radii.
- Modals, drawers, and larger detached container cards use up to 6px-8px (`rounded-lg`) maximum. Full-pill radii are avoided to preserve the disciplined, technical tool appearance.

## Components

### Buttons
- **Primary**: Background `#E65100`, text `#FFFFFF`, font-weight 500, height 36px (32px for compact table toolbars), padding 0 14px, radius 4px. Hover state: `#CC4800`. Active state: `#B23F00`.
- **Secondary**: Pure white background `#FFFFFF`, 1px solid border `#E0E0E0`, text `#212121`, font-weight 500. Hover state: border color `#D0D0D0`, background `#F5F5F5`. Active state: background `#EEEEEE`.
- **Destructive**: White background, 1px solid border `#FFCDD2`, text `#C62828`. Hover: `#FFEBEE`.

### Badges & Status Indicators
Rendered as inline-flex items, font size 11px, font-weight 600, padding 2px 8px, border-radius 4px, non-pill format:
- **Доступно**: Background `#E8F5E9`, text `#1B5E20`, border 1px solid transparent.
- **Недоступно / На руках**: Background `#F5F5F5`, text `#616161`, border 1px solid `#E0E0E0`.
- **В ремонте**: Background `#FFEBEE`, text `#C62828`, border 1px solid transparent.
- **Списано**: Background `#EEEEEE`, text `#757575`, border 1px solid transparent.

### Inputs & Select Fields
- Height 36px, background `#FFFFFF`, border 1px solid `#E0E0E0`, radius 4px, padding 0 10px, typography `body-md` (`#212121`).
- Hover: border `#BDBDBD`.
- Focus: border `#E65100`, outline 2px solid rgba(230, 81, 0, 0.2).
- Placeholder: `#9E9E9E`.

### Equipment Data Table
- Density: Compact (row height 40px to 44px).
- Header: Background `#F5F5F5`, text `#616161`, uppercase `label-sm`, bottom border 1px solid `#E0E0E0`.
- Cells: Bottom border 1px solid `#F0F0F0`, tabular numeric values for IDs, serials, and timestamps. Hover row background: `#FAFAFA`.

### Checkboxes & Radios
- Size 16x16px, border 1px solid `#BDBDBD`, radius 3px (checkbox) or circular (radio).
- Checked: Background `#E65100`, border `#E65100`, checkmark white.