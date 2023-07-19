# Erstelle ein ECS Cluster 



## # [Gehe zuAmazon ECS](https://eu-central-1.console.aws.amazon.com/ecs/v2/clusters/eddytest/services?region=eu-central-1)


### 1. Klicke auf Cluster erstellen
![Step 1 screenshot](https://images.tango.us/workflows/641e61ef-f28b-4791-99a1-7e3b7e6c153d/steps/891155bd-5ce0-4fb7-956e-63118ea6a0fa/f6776efc-dc0e-430d-9add-af51f5d10813.png?crop=focalpoint&fit=crop&fp-x=0.8604&fp-y=0.1702&fp-z=2.9216&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=487&mark-y=390&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00NDgmaD0xMTEmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 2. Geb dem Cluster einen Namen "TechstarterCluster"
![Step 2 screenshot](https://images.tango.us/workflows/641e61ef-f28b-4791-99a1-7e3b7e6c153d/steps/6586e83f-9831-4f3d-862e-c3e1f0919ba7/12a74b61-f904-45c6-a8a4-f0a9a9c28b6b.png?crop=focalpoint&fit=crop&fp-x=0.4909&fp-y=0.3805&fp-z=1.3605&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=231&mark-y=422&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz03MzgmaD01MiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 3. Wähle dein VPC aus
![Step 3 screenshot](https://images.tango.us/workflows/641e61ef-f28b-4791-99a1-7e3b7e6c153d/steps/fc2bfd8c-51c8-4262-aee7-d4ea2e7bef85/4367911a-27c4-494e-a978-6b5e02fd85bc.png?crop=focalpoint&fit=crop&fp-x=0.4909&fp-y=0.5909&fp-z=1.3605&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=231&mark-y=422&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz03MzgmaD01MiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 4. Lösche alle Privaten Subnets
![Step 4 screenshot](https://images.tango.us/workflows/641e61ef-f28b-4791-99a1-7e3b7e6c153d/steps/ca430747-f822-4060-935d-bbc3c724f92b/fdd164cc-4a4f-44a5-bf9c-8d4e17e6b196.png?crop=focalpoint&fit=crop&fp-x=0.6735&fp-y=0.7410&fp-z=3.0598&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=551&mark-y=401&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz05OCZoPTkzJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)


ℹ️ Natürlich löschen wir die Privaten Subnets nur für die Demo und nicht für echte Apps


### 5. Click on Erstellen
![Step 5 screenshot](https://images.tango.us/workflows/641e61ef-f28b-4791-99a1-7e3b7e6c153d/steps/14b4e809-eee0-4cb5-8c56-2567c6e1c8f4/5d8d7c92-a9d8-496b-8f7e-c1088891f0df.png?crop=focalpoint&fit=crop&fp-x=0.8431&fp-y=0.9313&fp-z=4.0000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=392&mark-y=574&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00MTYmaD0xNTEmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 6. Wenn du willst, kannst du dir die Clustererstellung in Cloudformation anschauen
![Step 6 screenshot](https://images.tango.us/workflows/641e61ef-f28b-4791-99a1-7e3b7e6c153d/steps/096cc3d5-873b-48e8-9bc0-8bb10416636d/940d2419-2096-494e-b5a5-d16571fa9e53.png?crop=focalpoint&fit=crop&fp-x=0.5946&fp-y=0.1004&fp-z=1.2782&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=22&mark-y=81&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0xMTU2Jmg9NjgmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)

<br/>
