> To create stunning animated gradient borders using Tailwind CSS to enhance your web design with vibrant colors and smooth transitions.


# Html
```html
<div class="h-screen flex  items-center justify-center bg-black ">
      <div class="
        bg-black 
        text-white 
        p-6 
        shadow-lg
        w-full 
        max-w-[422px] 
        [background:linear-gradient(45deg,#172033,theme(colors.slate.800)_50%,#172033)_padding-box,conic-gradient(from_var(--border-angle),theme(colors.slate.600/.48)_80%,theme(colors.indigo.500)_86%,theme(colors.indigo.300)_90%,theme(colors.indigo.500)_94%,theme(colors.slate.600/.48))_border-box] 
        rounded-2xl 
        border 
        border-transparent 
        animate-border
      ">
        <div class="text-2xl text-white font-bold">Your Mood</div>
      </div>
    </div>
    </div>
```

# CSS
```css

@tailwind base;
@tailwind components;
@tailwind utilities;
@property --border-angle {
  inherits: false;
  initial-value: 0deg;
  syntax: '<angle>';
}     
```
# Config

```text
theme: {
            extend: {
                animation: {
                    'border': 'border 4s linear infinite',
                },
                keyframes: {
                    'border': {
                        to: { '--border-angle': '360deg' },
                    }
                }                      
            },
        },
    };
```
