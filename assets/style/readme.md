Disable execution policy
Set-ExecutionPolicy -Scope Process RemoteSigned
.............................................................
to generated package.json file.
npm init -y
.................................................................
for install tailwind and dependency package.

npm install -D tailwindcss @tailwindcss/postcss postcss postcss-cli

.............................................
postcss.config.js

module.exports = {
  plugins: {
    "@tailwindcss/postcss": {},
  },
};


.............................
input.css
@import "tailwindcss";

  ...................................

run this command for generate compiled css file
npx postcss ./assets/style/input.css -o ./assets/style/main.css --watch
...................................