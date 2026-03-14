# CoreInventory - Odoo-Inspired Design System

## Overview

CoreInventory now features a complete visual overhaul inspired by Odoo 17/18's design language, emphasizing subtlety, professionalism, and high-fidelity user experience.

## Typography

- **Font Family**: Inter (Google Fonts)
- **Weights**: 300, 400, 500, 600, 700, 800
- **Usage**: Clean, formal, and highly readable across all interface elements

## Color Palette

### Primary Colors
- **Primary**: `#4f46e5` (indigo-600) - Professional indigo for primary actions
- **Primary Hover**: `#4338ca` (indigo-700)
- **Primary Light**: `#eef2ff` (indigo-50) - For backgrounds and subtle highlights

### Semantic Colors
- **Accent**: `#059669` (emerald-600) - Success states and positive actions
- **Warning**: `#d97706` (amber-600) - Warning states and pending items
- **Danger**: `#dc2626` (red-600) - Error states and critical alerts

### Neutral Colors
- **Background**: `#f8fafc` (slate-50) - Main application background
- **Text Primary**: `#0f172a` (slate-900) - Headings and primary text
- **Text Secondary**: `#64748b` (slate-500) - Secondary text and labels
- **Border**: `#e2e8f0` (slate-200) - Subtle borders and dividers

## Layout Components

### Sidebar
- **Background**: White with subtle right border
- **Width**: 256px (w-64)
- **Navigation**: Minimalist with 18px Lucide icons
- **Active State**: Indigo background tint with thick left border accent
- **Typography**: Clean section headers with proper spacing

### Topbar
- **Height**: 64px (h-16)
- **Background**: White with bottom border
- **Content**: Breadcrumb navigation and user controls
- **Notifications**: Clean bell icon with badge indicators

### Main Content
- **Background**: `slate-50` for subtle contrast
- **Padding**: 24px (p-6) for comfortable spacing
- **Layout**: Flexible grid system for responsive design

## Component Design

### Cards
- **Background**: White with subtle shadow (`shadow-subtle`)
- **Border**: Light slate border (`border-slate-200`)
- **Radius**: Extra large (`rounded-xl`)
- **Hover**: Enhanced shadow for interaction feedback
- **Padding**: Generous internal spacing (p-6 for KPI cards)

### Tables (Zebra Style)
- **Background**: White base with alternating row colors
- **Headers**: Uppercase, small font, slate-500 color
- **Borders**: Extremely light (`border-slate-100`)
- **Hover**: Subtle background change (`hover:bg-slate-50`)
- **Typography**: Consistent sizing and spacing

### Buttons

#### Primary Button
- **Background**: `bg-primary-600` with hover state
- **Height**: 36px (h-9) for consistent sizing
- **Typography**: Medium weight, white text
- **Focus**: Ring indicator for accessibility

#### Secondary Button
- **Background**: White with slate border
- **Hover**: Light slate background
- **Typography**: Slate-700 text

#### Ghost Button
- **Background**: Transparent
- **Hover**: Light slate background
- **Usage**: Tertiary actions and subtle interactions

### Form Controls

#### Input Fields
- **Height**: 36px (h-9) for consistency
- **Border**: Light slate with focus ring
- **Typography**: Slate-900 text, slate-400 placeholder
- **Focus**: Primary color ring and border

#### Select Fields
- **Styling**: Matches input fields
- **Icon**: Custom dropdown arrow
- **Background**: Right-positioned chevron icon

### Status Badges (Pastel Style)
- **Draft**: Light slate background with dark text
- **Waiting**: Light amber background with dark amber text
- **Ready**: Light primary background with dark primary text
- **Done**: Light emerald background with dark emerald text
- **Canceled**: Light red background with dark red text
- **Shape**: Pill-shaped with border for definition

### KPI Cards
- **Layout**: Icon in top-right corner with colored background
- **Typography**: Clear hierarchy with labels and values
- **Spacing**: Generous padding and line spacing
- **Hover**: Subtle shadow enhancement

### Summary Badges
- **Design**: Icon + label + value layout
- **Colors**: Semantic color backgrounds with matching text
- **Border**: Subtle border for definition
- **Hover**: Light shadow for interaction feedback

## Spacing System

- **Base Unit**: 4px (Tailwind's default)
- **Component Padding**: 24px (p-6) for cards and major sections
- **Element Spacing**: 16px (gap-4) between related elements
- **Section Spacing**: 24px (space-y-6) between major sections

## Shadow System

- **Subtle**: `shadow-subtle` - Minimal shadow for cards
- **Card**: `shadow-card` - Standard card shadow
- **Card Hover**: `shadow-card-hover` - Enhanced shadow on interaction

## Responsive Design

- **Breakpoints**: Standard Tailwind breakpoints
- **Grid**: Flexible grid system that adapts to screen size
- **Typography**: Consistent scaling across devices
- **Touch Targets**: Minimum 44px for mobile accessibility

## Accessibility Features

- **Focus Indicators**: Visible focus rings on all interactive elements
- **Color Contrast**: WCAG AA compliant color combinations
- **Typography**: Readable font sizes and line heights
- **Touch Targets**: Appropriate sizing for mobile devices

## Implementation Notes

### CSS Classes
- All components use utility-first Tailwind CSS
- Custom component classes defined in `@layer components`
- Consistent naming convention following BEM-like patterns

### Component Structure
- Modular component architecture
- Consistent prop interfaces
- Reusable design tokens

### Performance
- Optimized font loading with Google Fonts
- Efficient CSS with Tailwind's purging
- Minimal custom CSS for better maintainability

## Usage Guidelines

1. **Consistency**: Always use defined color tokens and spacing units
2. **Hierarchy**: Maintain clear visual hierarchy with typography and spacing
3. **Feedback**: Provide appropriate hover and focus states
4. **Accessibility**: Ensure all interactive elements are keyboard accessible
5. **Responsiveness**: Test components across different screen sizes

## File Structure

```
frontend/src/
├── index.css              # Global styles and component definitions
├── tailwind.config.js     # Tailwind configuration with custom tokens
├── components/
│   ├── layout/            # Layout components (Sidebar, Topbar, AppLayout)
│   ├── ui/                # Reusable UI components
│   └── dashboard/         # Dashboard-specific components
└── pages/                 # Page components with consistent styling
```

This design system ensures a cohesive, professional, and user-friendly interface that scales well across the entire CoreInventory application.