# be_nappier
Multifunctional Whatsapp bot 🪐 with advanced features 📯 leave a ⭐ and fork repo
@tailwind base;
@tailwind components;
@tailwind utilities;

/* Definition of the design system. All colors, gradients, fonts, etc should be defined here. 
All colors MUST be HSL.
*/

@layer base {
  :root {
    --background: 240 10% 3.9%;
    --foreground: 180 100% 90%;

    --card: 240 10% 7%;
    --card-foreground: 180 100% 90%;

    --popover: 240 10% 7%;
    --popover-foreground: 180 100% 90%;

    --primary: 166 100% 50%;
    --primary-foreground: 240 10% 3.9%;

    --secondary: 270 95% 65%;
    --secondary-foreground: 240 10% 3.9%;

    --muted: 240 10% 15%;
    --muted-foreground: 180 50% 60%;

    --accent: 142 76% 36%;
    --accent-foreground: 180 100% 90%;

    --destructive: 0 84.2% 60.2%;
    --destructive-foreground: 210 40% 98%;

    --border: 240 10% 15%;
    --input: 240 10% 15%;
    --ring: 166 100% 50%;

    --radius: 0.75rem;

    --terminal-glow: 166 100% 50%;
    --terminal-shadow: 0 0 20px hsl(var(--terminal-glow) / 0.3);
  }
}

@layer base {
  * {
    @apply border-border;
  }

  body {
    @apply bg-background text-foreground font-mono;
    background: linear-gradient(to bottom, hsl(240 10% 3.9%), hsl(240 10% 6%));
    min-height: 100vh;
  }

  h1, h2, h3, h4, h5, h6 {
    @apply font-bold;
  }

  .terminal-glow {
    text-shadow: 0 0 10px hsl(var(--terminal-glow) / 0.5);
  }

  .card-glow {
    box-shadow: 0 0 20px hsl(var(--terminal-glow) / 0.1);
  }
}
