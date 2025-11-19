
Beadandó csomag – Online Éttermi Rendelés és Futárkövetés

Tartalom:
- Rendszerleiras_online_ettermi_rendeles.docx  → minimum fél A/4 oldal leírás a rendszer elvárt működéséről.
- osztalydiagram.puml                         → PlantUML osztálydiagram forrás.
- usecase_diagram.puml                        → PlantUML használati eset diagram.
- aktivitas_diagram.puml                      → PlantUML aktivitásdiagram.

Hogyan exportálj PNG/SVG képeket a .puml fájlokból (bármelyik opció jó):
1) https://www.plantuml.com/plantuml/ (szerkesztő) → a kód beillesztése → Export PNG/SVG.
2) VS Code + "PlantUML" kiegészítő → megnyitod a .puml-t → jobb klikk: "Export Current Diagram".
3) Helyi PlantUML/Graphviz: 
   java -jar plantuml.jar osztalydiagram.puml
   java -jar plantuml.jar usecase_diagram.puml
   java -jar plantuml.jar aktivitas_diagram.puml

Mit ellenőrizz még a feltöltés előtt (értékelési szempontok szerint):
- Osztálydiagram: elegendő osztály, enumerációk (RendelesAllapot, FizetesMod, stb.), asszociációk, öröklés, kompozíciók, UI ablakokhoz dependency.
- Use Case: aktorok (Vásárló, Futár, Admin, PSP), include/extend, aktor‑kapcsolatok.
- Aktivitás: kezdő/végpont, döntések, kupon ági elágazás, szinkronizáció (fork/join), „úszósávok” (swimlane-ek).

Tippek a Coospace feltöltéshez:
- A .puml képekből generálj PNG-ket, és egy mappában add le (vagy a forrásokat is mellékelheted).
- Tedd mellé a .docx rendszerleírást és – ha szükséges – egy rövid „csapatszerepek.txt”-t.
