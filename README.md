## Steps to reproduce ##
1. Build and run
    1. `npm install`
    2. `npm run dev`
    3. Open http://localhost:3000 in your browser
2. In `src/App.vue`, change `bg-red-600` to `bg-blue-600` (or make some other class change)\
You should see the class update in your html but the color goes blank instead of turning blue.
3. Go to `src/tailwind.css` and save the file. You should see the changes expected in step 2.

Now remove `base: "/static",` from `vite.config.js` and repeat the above test. You should see it work correctly.
