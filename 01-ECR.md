# Erstelle ein ECR Repository und pushe ein lokales Docker image zu AWS
***

## # [Elastic Container Registry - Repositories](https://eu-central-1.console.aws.amazon.com/ecr/repositories?region=eu-central-1)
Gehe zu ECR in AWS


### 1. Übersicht
![Step 1 screenshot](https://images.tango.us/workflows/71f6d733-c94a-413b-8621-b1c7b93cfdef/steps/b91ca207-c2f6-4cc7-9b18-06769010f645/48d207e1-6ba8-40d8-b0f2-19a66e7489ef.png?crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n)


### 2. Klicke auf Repository erstellen
![Step 2 screenshot](https://images.tango.us/workflows/71f6d733-c94a-413b-8621-b1c7b93cfdef/steps/851f4fc4-7e1f-4d43-a117-45a563319f3c/95c17cfc-f621-40ec-a91e-f4548fe763ec.png?crop=focalpoint&fit=crop&fp-x=0.7837&fp-y=0.3593&fp-z=2.8551&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=329&mark-y=344&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz01NDImaD0xMTUmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 3. Stelle sicher, dass die Einstellungen auf Privat stehen
![Step 3 screenshot](https://images.tango.us/workflows/71f6d733-c94a-413b-8621-b1c7b93cfdef/steps/25a209cc-d4d2-45a1-842b-9474407c9963/d0450732-2582-4d03-a8a0-ff4c342a037a.png?crop=focalpoint&fit=crop&fp-x=0.3220&fp-y=0.4447&fp-z=1.2782&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=124&mark-y=343&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz03NDAmaD0xMTkmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 4. Gib dem Repo einen Namen
![Step 4 screenshot](https://images.tango.us/workflows/71f6d733-c94a-413b-8621-b1c7b93cfdef/steps/a519102a-685e-484f-a491-acf35c5089cc/339c8e8a-6961-459a-859b-66983b30a579.png?crop=focalpoint&fit=crop&fp-x=0.5337&fp-y=0.6005&fp-z=1.5959&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=287&mark-y=370&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz02MjUmaD02NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 5. Klick auf Repository erstellen
![Step 5 screenshot](https://images.tango.us/workflows/71f6d733-c94a-413b-8621-b1c7b93cfdef/steps/0ea347a2-1bf3-41ab-b4b2-cad175cfe59e/8edc67b4-eb1b-4789-ab1c-5ef5dc17a0c4.png?crop=focalpoint&fit=crop&fp-x=0.6650&fp-y=0.9158&fp-z=2.4146&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=371&mark-y=592&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00NTkmaD05OCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 6. Klicke auf dein neu erstelltes Repository
![Step 6 screenshot](https://images.tango.us/workflows/71f6d733-c94a-413b-8621-b1c7b93cfdef/steps/cb31175f-3cb3-454e-9da3-601d7f5383f8/0fd3f17b-fab7-4379-9e97-dddd4c28f8ad.png?crop=focalpoint&fit=crop&fp-x=0.3577&fp-y=0.8499&fp-z=2.7861&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=502&mark-y=433&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0xOTcmaD03MCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 7. Klicke auf Push-Befehle anzeigen
![Step 7 screenshot](https://images.tango.us/workflows/71f6d733-c94a-413b-8621-b1c7b93cfdef/steps/7f0a036e-63b4-4f5e-a0c5-57475feeeefa/7e460371-c3cd-4997-98a6-7dc6f404c597.png?crop=focalpoint&fit=crop&fp-x=0.7786&fp-y=0.1922&fp-z=2.8551&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=303&mark-y=344&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz01OTQmaD0xMTUmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 8. Klicke auf Windows
![Step 8 screenshot](https://images.tango.us/workflows/71f6d733-c94a-413b-8621-b1c7b93cfdef/steps/76e14639-3604-4592-ac6f-3b114e6871fa/899d9c3d-6bd7-4a52-a759-5cae6f8d5765.png?crop=focalpoint&fit=crop&fp-x=0.3245&fp-y=0.1539&fp-z=2.5526&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=459&mark-y=235&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0yODEmaD0xNjImZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 9. Öffne deinen Terminal und kopiere deinen AWS Access Key und ID für in den Terminal, somit bist du bei AWS in deiner Konsole angemeldet und der nächste Schritt wird funktionieren.
Teste die Verbindung im selben Terminal mit "aws s3 ls"
![Step 9 screenshot](https://images.tango.us/workflows/71f6d733-c94a-413b-8621-b1c7b93cfdef/steps/8d83b87a-d4ae-4880-935f-f0b2e828de3e/044f4978-aa05-4a46-b465-8339e58944a2.png?crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n)


### 10. Folge den Befehlen um deinen Docker Container zu ECR zu pushen
![Step 10 screenshot](https://images.tango.us/workflows/71f6d733-c94a-413b-8621-b1c7b93cfdef/steps/fa46be8c-f458-4025-a276-730a09b7c8ef/26ffc51a-67bc-4aab-829d-36b8bc3446bf.png?crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5389&fp-z=1.2024&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=121&mark-y=77&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz05NTcmaD02NTEmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 11. Hat alles geklappt wirst du dein Image hier finden.
![Step 11 screenshot](https://images.tango.us/workflows/71f6d733-c94a-413b-8621-b1c7b93cfdef/steps/c24a1e7c-de3e-4124-980c-fdab867203f5/66c85993-0569-4cda-8d9f-0e51f7d33871.png?crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n)

<br/>

