# Interactive Client Acquisition Network Visualizer

A responsive, interactive network visualization component that demonstrates client acquisition as an interconnected web system. Built for seamless Webflow integration with React, TypeScript, D3.js, and Framer Motion.

## 🎯 Overview

This visualizer showcases the power of networked client acquisition systems versus traditional linear funnels. It features 15 interconnected touchpoints across acquisition, tracking, analytics, optimization, and automation categories.

## ✨ Features

- **Interactive Physics Simulation**: D3.js force simulation with drag-and-drop nodes
- **Modern Design**: Outlined rectangular nodes with subtle brand-colored glows
- **Roboto Typography**: Clean sans-serif font with tier-based weights
- **Smart Connectors**: Lines connect precisely to node edges, not centers
- **Responsive Design**: Seamless adaptation from mobile to desktop
- **Animated Connections**: Flowing data connections with pulse animations
- **Brand Compliance**: Salt Lick Denver color scheme and typography
- **Accessibility**: WCAG AA compliant with keyboard navigation
- **Webflow Ready**: Drop-in integration with auto-initialization

## 🚀 Quick Start

### Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```

### Webflow Integration

1. **Include React dependencies** in your Webflow page:
```html
<script crossorigin src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
```

2. **Add container element**:
```html
<div id="network-visualizer" 
     data-theme="saltlick" 
     data-responsive="true" 
     data-autoplay="true"
     style="width: 100%; height: 600px;">
</div>
```

3. **Include the bundle**:
```html
<script src="path/to/network-visualizer.umd.js"></script>
```

## 🎨 Design System

### Node Design
- **Shape**: Thin rectangular nodes optimized for text readability
- **Styling**: Transparent background with brand-colored outlines
- **Glows**: Subtle brand-colored shadows that intensify on interaction
- **Typography**: Roboto sans-serif with tier-based font weights

### Connection System
- **Particle Streams**: Animated particles flow between connected nodes instead of static lines
- **Real-time Tracking**: Particles automatically follow nodes during drag operations
- **Edge Connections**: Particles spawn from and travel to precise node edge points
- **Dynamic Animation**: Particles continuously spawn, travel, and fade for living connections
- **Performance Optimized**: RequestAnimationFrame-based animation with efficient particle management
- **Responsive Intensity**: More particles and faster spawning when nodes are highlighted
- **Bezier Paths**: Particles follow curved trajectories for natural, organic movement
- **Category Colors**: Each particle stream uses the source node's brand color

## 🎨 Network Architecture

### Node Tiers
- **Primary (3 nodes)**: Ad Creative, Conversions API, Server Side Tracking
- **Secondary (7 nodes)**: Attribution, Custom Conversions, Event Targeting, etc.
- **Tertiary (5 nodes)**: Estimate Generation, Scheduling, Follow-up, etc.

### Categories
- **Acquisition**: Primary touchpoints for customer acquisition
- **Tracking**: Data collection and measurement systems  
- **Analytics**: Data analysis and attribution systems
- **Optimization**: Conversion and targeting improvements
- **Automation**: AI-driven sales and admin processes
- **Sales**: Direct customer interaction points
- **Fulfillment**: Service delivery and invoicing

## 🛠️ Configuration

```typescript
interface NetworkVisualizerProps {
  theme?: 'saltlick' | 'default';
  responsive?: boolean;
  autoplay?: boolean;
  className?: string;
}
```

### Data Attributes
- `data-theme`: Theme selection
- `data-responsive`: Enable responsive behavior
- `data-autoplay`: Enable auto-reheat simulation

## 📦 Build Output

- `dist/network-visualizer.umd.js` - UMD bundle for browsers (~370KB, gzipped: ~120KB)
- `dist/network-visualizer.es.js` - ES module bundle
- `dist/index.d.ts` - TypeScript definitions
- Source maps included for debugging

## 🔧 Development Scripts

```bash
npm run dev          # Development server (localhost:5173)
npm run build        # Production build
npm run typecheck    # TypeScript validation
npm run lint         # ESLint checking
npm run preview      # Preview built files
```

## 📱 Responsive Breakpoints

- **Mobile**: < 768px (simplified interactions)
- **Tablet**: 768px - 1199px (scaled nodes)  
- **Desktop**: ≥ 1200px (full feature set)

## ♿ Accessibility

- **WCAG AA Compliant**: Proper color contrast and focus states
- **Keyboard Navigation**: Tab/Arrow key support
- **Screen Reader**: ARIA labels and descriptions
- **Motion Respect**: Honors prefers-reduced-motion

Built with ❤️ for modern client acquisition visualization
