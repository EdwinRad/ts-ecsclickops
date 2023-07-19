# Erstelle ein Ngnix ECS Task

## # [Amazon ECS](https://eu-central-1.console.aws.amazon.com/ecs/v2/clusters/TechstarterCluster/services?region=eu-central-1)


### 1. In ECS klicke auf Aufgabendefinitionen
![Step 1 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/6bfeca0f-a7ae-49ac-b029-1d77d49a41c7/630b9f3f-3902-46d5-9016-2a1509a237b5.png?crop=focalpoint&fit=crop&fp-x=0.0800&fp-y=0.3346&fp-z=2.4042&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=64&mark-y=419&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0zMzQmaD01NyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 2. Klicke auf Neue Aufgabendefinition erstellen
![Step 2 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/49015ab1-d08b-43d8-a10e-958cc78c7b61/2da9d5e6-66e8-461e-8d89-b8096af2064a.png?crop=focalpoint&fit=crop&fp-x=0.7528&fp-y=0.2928&fp-z=2.6091&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=174&mark-y=401&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz04NTImaD05NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 3. Namen
![Step 3 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/07435f36-b169-48d0-882c-1095699cd1a8/ee822c26-6c0a-4de0-be9b-27a492e0cb69.png?crop=focalpoint&fit=crop&fp-x=0.6991&fp-y=0.4355&fp-z=1.9448&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=102&mark-y=411&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz05OTYmaD03NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 4. Gebe hier einfach einen Namen ein
![Step 4 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/19df22f6-7d46-4ad9-86b2-33788d33fe9a/1707045a-579c-41ff-9a7b-3ba7202d938b.png?crop=focalpoint&fit=crop&fp-x=0.5355&fp-y=0.3488&fp-z=2.5039&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=451&mark-y=400&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0yOTkmaD05NSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 5. Für die Image Uri musst du zurück zu ECR 
![Step 5 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/20b3b8c0-97b8-478c-b2cf-bf8457697a1b/8fe3bd73-7c8b-4e54-aa09-5302ad31eb6f.png?crop=focalpoint&fit=crop&fp-x=0.6991&fp-y=0.3488&fp-z=2.4669&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=291&mark-y=401&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz02MTkmaD05MyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 6. Type "ecr"
![Step 6 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/4a2d5724-0a88-4243-add5-2167a1cee6f2/2f67b8d9-9a51-4574-a4e8-d0462939279b.png?crop=focalpoint&fit=crop&fp-x=0.3470&fp-y=0.0243&fp-z=1.3658&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=215&mark-y=5&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz03MDgmaD00OSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 7. Kopiere die URI für dein Repo
![Step 7 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/69cb887f-35cc-4438-a8a3-9cd6733589e7/3f6f6a43-d8b5-4200-9ea9-560bf0e334aa.png?crop=focalpoint&fit=crop&fp-x=0.4259&fp-y=0.7474&fp-z=3.0598&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=551&mark-y=390&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz05OCZoPTExNiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 8. Und hier rein kopieren
![Step 8 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/cef18ed8-2171-4550-bc59-9924e5173e9d/4cae71d3-707f-42b7-a621-eacc5a0aa991.png?crop=focalpoint&fit=crop&fp-x=0.6991&fp-y=0.3488&fp-z=2.4669&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=291&mark-y=401&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz02MTkmaD05MyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 9. Nächster Schritt
![Step 9 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/d4ef5690-61a1-420c-bc3f-984fdbdadb9c/5a082563-ba74-43dc-bd9e-f1965fdb0793.png?crop=focalpoint&fit=crop&fp-x=0.8651&fp-y=0.9292&fp-z=4.0000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=297&mark-y=566&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz02MDYmaD0xNTEmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 10. Ngnix braucht so praktisch keine Resourcen also wähle: .25 vCPU…
![Step 10 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/58748ab3-60ae-485c-b697-d6a932068708/edeb7007-23b3-415f-949a-4fa202400a5c.png?crop=focalpoint&fit=crop&fp-x=0.5844&fp-y=0.6247&fp-z=2.0114&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=362&mark-y=394&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00NzYmaD0xMDcmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 11. Und .5 GB…
![Step 11 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/276bf2c7-2138-4435-8fa9-2c313618c29e/e31e98eb-ec73-424e-b235-66a0930d2eb0.png?crop=focalpoint&fit=crop&fp-x=0.8028&fp-y=0.5973&fp-z=2.7840&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=271&mark-y=374&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz02NTkmaD0xNDgmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 12. Wähle die ecsTaskExecutionRole oder erstelle eine passende Rolle
![Step 12 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/88d0ce4f-99e2-4ee5-bb0f-9233449b70e6/8f5c5f7c-38b2-4dbe-9750-b3b5046809e0.png?crop=focalpoint&fit=crop&fp-x=0.5903&fp-y=0.7230&fp-z=1.9647&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=354&mark-y=410&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00OTMmaD03NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 13. Protokollerfassung brauchen wir für den Anfang nicht
![Step 13 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/99e970c9-66ac-4b2d-830c-d4d2a7c824b9/c803a04c-ec92-417d-b537-ddc428a3c62d.png?crop=focalpoint&fit=crop&fp-x=0.4945&fp-y=0.5085&fp-z=3.0935&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=568&mark-y=415&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz02NCZoPTY0JmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)


### 14. Nächster Schritt
![Step 14 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/412ddbd6-e648-4edb-80f0-2272dbfa423f/d3d376fb-eb77-4e38-ae0b-1800b25c95bf.png?crop=focalpoint&fit=crop&fp-x=0.8651&fp-y=0.9292&fp-z=4.0000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=297&mark-y=566&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz02MDYmaD0xNTEmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 15. In der Benachrichtigung wähle Bereitstellen und Service erstellen
![Step 15 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/cc577b58-6ace-44a8-80db-4f4967403c5c/53ed97d8-744d-4f38-bccd-166e53b3d4d2.png?crop=focalpoint&fit=crop&fp-x=0.8699&fp-y=0.1871&fp-z=2.9397&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=485&mark-y=395&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz01MTImaD0xMDYmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 16. Wähle dein Cluster
![Step 16 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/72e02b0e-4174-4f7a-ba23-e62a3980c4f8/5ed41d13-b589-4ac3-9dc0-665915c7750b.png?crop=focalpoint&fit=crop&fp-x=0.4909&fp-y=0.4313&fp-z=1.3605&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=231&mark-y=422&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz03MzgmaD01MiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 17. Wähle Starttyp
![Step 17 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/7375a18e-02d9-4279-b486-90026d7c5870/ead1a3bd-545d-485c-b02d-c4d3917027fa.png?crop=focalpoint&fit=crop&fp-x=0.5181&fp-y=0.5645&fp-z=3.0935&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=568&mark-y=415&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz02NCZoPTY0JmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)


### 18. FARGATE aka Serverless
![Step 18 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/3ac6e40b-27af-4802-b282-3b4b22488df9/9eee195e-66ef-4f0b-bc5a-c1f8b9d0ae5d.png?crop=focalpoint&fit=crop&fp-x=0.3178&fp-y=0.6543&fp-z=2.4650&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=444&mark-y=401&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0zMTMmaD05MyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 19. Type "TSService"
![Step 19 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/4331da1f-fc70-4c76-9c40-bbb3366ac4b5/dec708cd-5412-4e1d-9047-92e455e9ae6a.png?crop=focalpoint&fit=crop&fp-x=0.4909&fp-y=0.5634&fp-z=1.3605&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=231&mark-y=422&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz03MzgmaD01MiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 20. Erstellen
![Step 20 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/10ccf5c3-1f6f-4862-808f-d5b10d1df03a/d526946a-59f9-4124-9c2a-2b07d1f84482.png?crop=focalpoint&fit=crop&fp-x=0.8431&fp-y=0.9292&fp-z=4.0000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=392&mark-y=566&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00MTYmaD0xNTEmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 21. Zeit für eine mini Pause, dauert ein paar Minuten, wenn fertig dann klicke auf neuladen
![Step 21 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/a90e5f17-66aa-47bf-9ed1-fd735d2075eb/bdd9cf0f-3383-4019-a39d-fe3f486796c3.png?crop=focalpoint&fit=crop&fp-x=0.4479&fp-y=0.8023&fp-z=2.8923&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=521&mark-y=393&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0xNTkmaD0xMDkmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 22. Wähle deinen Service
![Step 22 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/c9ace0fc-ccc1-434e-8bf8-1e24d7b64399/283e5750-3254-4d35-894f-1be2420bf98f.png?crop=focalpoint&fit=crop&fp-x=0.3348&fp-y=0.8800&fp-z=2.8215&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=508&mark-y=559&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0xODQmaD02NyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 23. Click on Aufgaben
![Step 23 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/b8ba2ea3-ab3a-4986-abdf-4abceb37cc6c/36b2955d-10fe-487a-912a-d549cfa42ae5.png?crop=focalpoint&fit=crop&fp-x=0.4692&fp-y=0.2468&fp-z=2.5647&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=462&mark-y=371&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0yNzcmaD0xNTMmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 24. Und dann auf den Aufgabennamen
![Step 24 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/fd02a94e-bf89-4edb-b75c-2a1687ad0d9a/99756bd8-26d3-4212-a837-a02ccfc4cb5b.png?crop=focalpoint&fit=crop&fp-x=0.4267&fp-y=0.5629&fp-z=1.9987&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=360&mark-y=424&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00ODAmaD00NyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 25. Unter Netzwerke findest du hier die Öffentliche IP
![Step 25 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/7a055ab4-1dbc-4c8d-9993-b84af06ac787/ad0dce77-2109-46a0-af44-d50c566b1cac.png?crop=focalpoint&fit=crop&fp-x=0.8482&fp-y=0.3473&fp-z=2.8597&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=450&mark-y=384&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00NTcmaD0xMjcmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 26. Welcome to nginx!
![Step 26 screenshot](https://images.tango.us/workflows/ae224e6d-13d4-4f99-b721-cf4e6a0e8fd7/steps/1495f69a-6dcf-4857-8cff-4184b604b553/71c9e1f9-699d-4fee-a291-832586b4e9a9.png?crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.1062&fp-z=1.3813&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=229&mark-y=101&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz03NDImaD02MSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


ℹ️ Lösche jetzt wieder die laufende Aufgabe!
