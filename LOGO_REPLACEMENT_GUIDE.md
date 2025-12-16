# Logo Replacement Guide for Alnex.ai

This guide lists all the files and locations where the Open WebUI logo needs to be replaced with the new Alnex.ai logo.

## Image Files to Replace

Replace the following image files in the `static/` directory with your new Alnex.ai logo:

### Favicon Files

1. `static/favicon.png` - Main favicon
2. `static/static/favicon.png` - Duplicate favicon location
3. `static/static/favicon.svg` - SVG favicon (vector format)
4. `static/static/favicon.ico` - ICO favicon (for older browsers)
5. `static/static/favicon-96x96.png` - 96x96 pixel favicon
6. `static/static/favicon-dark.png` - Dark mode favicon

### Splash Screen & Logo Files

7. `static/static/splash.png` - Main splash screen logo
8. `static/static/splash-dark.png` - Dark mode splash screen logo
9. `static/static/logo.png` - General logo file

### PWA & Mobile Icons

10. `static/static/apple-touch-icon.png` - Apple touch icon (180x180)
11. `static/static/web-app-manifest-192x192.png` - PWA icon 192x192
12. `static/static/web-app-manifest-512x512.png` - PWA icon 512x512

## Code References (No changes needed - these reference the files above)

The following files reference the logo files but don't need code changes - they'll automatically use the new files once you replace them:

- `src/app.html` - References favicon.png, splash.png
- `src/routes/auth/+page.svelte` - References favicon.png
- `src/routes/+layout.svelte` - References favicon.png
- `src/lib/components/app/AppSidebar.svelte` - References splash.png, favicon.png
- `src/lib/components/layout/Sidebar.svelte` - References favicon.png
- And other component files

## Recommended Sizes

For best results, create your logo in these sizes:

- **Favicon**: 32x32, 96x96, 192x192, 512x512 pixels
- **Splash screen**: 512x512 or larger (will be scaled)
- **Apple touch icon**: 180x180 pixels
- **SVG**: Vector format for scalability

## Steps to Replace

1. Create your Alnex.ai logo in the required sizes
2. Replace all the files listed above
3. Clear browser cache and hard refresh (Ctrl+Shift+R or Cmd+Shift+R)
4. Test in both light and dark modes
