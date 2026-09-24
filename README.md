# Chemical Equation Balancer

A comprehensive, interactive web application designed to balance chemical equations and provide step-by-step mathematical explanations. Built with modern web technologies, this tool helps students, educators, and chemists quickly solve chemical equations while understanding the underlying principles.

## Overview

The Chemical Equation Balancer uses a mathematical approach (Gaussian elimination) to solve complex chemical equations. It offers an intuitive two-column responsive interface where users can type in any unbalanced equation and instantly receive the balanced formula along with a detailed breakdown of the steps.

## Key Features

- **Instant Equation Balancing**: Accurately balances chemical equations in real-time.
- **Step-by-Step Explanations**: Provides clear, logical steps detailing the balancing process.
- **Interactive UI**: A sleek two-column layout that adapts beautifully to both mobile and desktop screens.
- **Dark Mode Support**: Built-in toggle for a comfortable viewing experience in low-light environments.
- **Equation History**: Automatically saves your recently balanced equations to local storage.
- **Export Options**: Export the balanced equations as PDF, PNG, JSON, or LaTeX.
- **Shareable Links**: Generate URLs to share specific equations easily with others.
- **Predefined Examples**: Includes common examples like combustion, synthesis, and decomposition reactions to help you get started quickly.

## Technologies Used

This project is built using a modern frontend stack to ensure high performance and maintainability:

- **React 18**: For building a dynamic and responsive user interface.
- **TypeScript**: Ensures type safety and better developer experience.
- **Vite**: A lightning-fast build tool and development server.
- **Tailwind CSS**: Utility-first CSS framework for rapid and responsive styling.
- **Radix UI**: Unstyled, accessible UI components (Accordion, Separator, Dialog, Dropdown Menu).
- **Framer Motion**: For fluid animations and transitions.
- **shadcn/ui**: High-quality, reusable component architecture.
- **Math.js**: Powerful mathematical logic engine for matrix calculations (Gaussian elimination).

## Getting Started

Follow these instructions to set up the project locally on your machine.

### Prerequisites

Ensure you have Node.js and npm installed on your system.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Dr-Rank1/Chemical-Equation.git
   ```
2. Navigate into the project directory:
   ```bash
   cd Chemical-Equation
   ```
3. Install the dependencies:
   ```bash
   npm install
   ```

### Development

To start the local development server:

```bash
npm run dev
```

The application will be accessible at `http://localhost:5173`. Any changes you make will be reflected instantly thanks to Vite's Hot Module Replacement (HMR).

### Production Build

To build the application for production:

```bash
npm run build
```

This command compiles the TypeScript code and bundles the application, optimizing it for production deployment. The output will be located in the `dist` directory.

To preview the production build locally:

```bash
npm run preview
```

## How It Works

The core of this application relies on linear algebra to balance equations. 
1. The app parses the chemical formula on the reactant and product sides.
2. It constructs a system of linear equations representing the conservation of mass for each element.
3. Using Gaussian elimination, it solves the system to find the smallest integer coefficients.
4. Finally, it normalizes the coefficients and formats the result for display.

## Author

Created and maintained by Ian Gicheha Mbae (Dr-Rank1).
