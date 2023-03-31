# customBahnhofstafel
a reverse-engineered Version of the web station sign in german train stations for use in workadveture

## installation

paste the customBahnhofstafel-Folder in the Folder:
```
./src/
```

and the station_sign_files/content.json and station_sign_files/Logo.gif in:
```
./public/src/customBahnhofstafel/station_sign_files/
```

in the vite.cofig.ts add the following line:

```
export default defineConfig({
  build: {
        rollupOptions: {
            input: {
              ...
                customBahnhofstafel: "./src/customStationSign/index.html",
              ...
```

## note

the content.json is not yet documented but it should be self explaitory

## usage

vite hosts the customBahnhofstafel in your github-pages with your project.
you can access it by implemeting it in an iFrame or typing:

```
https://<your-github-pages>/<your-project>/src/customBahnhofstafel/
```

## todo

- document the content.json