# ionic-vercel-local-function-testing
Sample project to demonstrate issues with running vercel dev to test vercel cloud functions on a local machine via localhost

* This is a standard ionic angular app created using "ionic start".  
* I've added a single hello.ts function under /api and deployed to vercel.
* Now I want to test locally using "ionic serve" and I want to run the vercel functions under /api locally with "vercel dev".

## Issue #1
Running "vercel dev" in the project folder for the first time gives the error "The specified command ("start") is invalid" see below:
```
vercel dev
Vercel CLI 21.3.3 dev (beta) — https://vercel.com/feedback
? Set up and develop “~/dev/ionic-vercel-local-function-testing”? [Y/n] y
? Which scope should contain your project? burggraf
? Link to existing project? [y/N] n
? What’s your project’s name? ionic-vercel-local-function-testing
? In which directory is your code located? ./
Auto-detected Project Settings (Ionic Angular):
- Build Command: `npm run build` or `ng build`
- Output Directory: www
- Development Command: ng start
? Want to override the settings? [y/N] n
🔗  Linked to burggraf/ionic-vercel-local-function-testing (created .vercel and added it to .gitignore)
> Running Dev Command “ng start”
The specified command ("start") is invalid. For a list of available options,
run "ng help".

Did you mean "test"?

```
## Issue #2
* What should the Dev Command be?
* How do I run "ionic serve" to test the front-end on port 8100 (the standard ionic test setup) and run vercel dev on another port to test the local functions?

