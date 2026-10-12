# LAILA x IT Resolver - web copy

Built from overlay_v2.html for the base URL: https://laila-film.ratha.dev/

1. Upload this whole folder so that index.html sits at that URL (keep the folder names).
   The host must send `Access-Control-Allow-Origin: *` (the page draws the icons and videos into WebGL).
   Cloudflare Pages and Netlify read the `_headers` file; Apache reads `.htaccess`; GitHub Pages and jsDelivr send it by default.
   Current host: GitHub Pages at https://laila-film.ratha.dev/ from the public repo rathahin/laila-film-web (push the folder to its main branch; DNS CNAME laila-film -> rathahin.github.io lives in Cloudflare, zone ratha.dev).
2. In Spline: open the file "Laila x Resolver", Code tab, paste index.html as the HTML content, then Export > Public URL.
   The 3D version lives at that Spline URL. Opening index.html directly on the host gives the flat version (no 3D bridge).
3. The saved Act 6 layout is embedded in index.html. Rebuild (python3 build_web.py --base ...) after changing the layout or the film.
