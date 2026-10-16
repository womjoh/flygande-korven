# Flygande Korven

En första övning i HTML, lokal utveckling och ett enkelt Git-flöde.

Du får menytexten, restaurangens logotyp och en tom CSS-fil. Du ska göra om texten till en strukturerad webbsida. Vi börjar lokalt under lektion 1 och använder GitHub Desktop under lektion 2.

## Lektion 1 — hämta filerna och skriv HTML

Till första lektionen behöver du **Visual Studio Code** och **Google Chrome**. GitHub Desktop och ditt GitHub-konto använder vi på andra lektionen. Du behöver inga terminalkommandon eller någon separat Git-installation för övningen.

### Förbered VS Code och Live Server

1. Starta VS Code.
2. Öppna **Extensions** och sök efter `Live Server`.
3. Installera **Live Server** av **Ritwick Dey**.
4. Starta Chrome. Nu är verktygen redo innan du hämtar projektet.

### 1. Hämta startmaterialet från kursens Google Drive

1. Öppna [Underlagsfiler till DD26](https://drive.google.com/drive/folders/1VJpyU_E2xTai6NmyjZNZtn3rgniVHLG6).
2. Ladda ned **flygande-korven.zip** till din dator.
3. Packa upp ZIP-filen.
4. Flytta den uppackade mappen `flygande-korven` till en plats du hittar igen, exempelvis Dokument.
5. Öppna VS Code och välj **File → Open Folder**. Välj mappen `flygande-korven`.
6. Om VS Code frågar om du litar på innehållet: kontrollera att det är kursens startmaterial och godkänn.

Vi hämtar startfilerna från Google Drive under lektion 1. Du behöver inget GitHub-konto den här dagen.

I **Explorer** ska du se `README.md`, `menu.txt`, `index.html`, `style.css` och mappen `assets`. Om du bara ser ytterligare en projektmapp har du öppnat mappen en nivå för högt. Öppna mappen där `index.html` ligger.

Arbeta i den uppackade mappen. Behåll samma projektmapp till lektion 2.

### 2. Visa sidan i Chrome

Live Server visar din lokala sida i webbläsaren och uppdaterar den när du sparar.

1. Öppna `index.html` och klicka på **Go Live** längst ner i VS Code. Du kan också högerklicka på filen och välja **Open with Live Server**.
2. Om en annan webbläsare öppnas: kopiera adressen till Chrome. Adressen börjar med `http://127.0.0.1` eller `http://localhost`.
3. I `index.html`: markera hela kommentaren som börjar med `<!--` och slutar med `-->`, inklusive båda teckenparen och alla rader mellan dem. Behåll resten av filen.
4. Skriv `Hej världen` för att ersätta allt du markerat. Du behöver inga nya HTML-taggar i detta första steg.
5. Spara med **Cmd + S** på Mac eller **Ctrl + S** på Windows och kontrollera att texten syns i Chrome. Ändra till en egen hälsning, spara och kontrollera igen.

**Om Live Server inte fungerar:** öppna `index.html` direkt i Chrome. Spara i VS Code och ladda sedan om sidan i Chrome efter varje ändring. Det fungerar för den här HTML/CSS-övningen.

### 3. Märk upp menyn

Utgå från [`menu.txt`](menu.txt) och bygg sidan i [`index.html`](index.html). Prova själv med stöd av lektionens exempel. Använd ingen kodagent för den första HTML-övningen.

- Använd HTML-element som passar innehållet.
- Skapa en begriplig rubrikstruktur.
- Presentera menyn som en lista eller beskrivningslista.
- Märk upp telefonnummer, öppettider och kontaktuppgifter tydligt.
- Lägg till logotypen från `assets/flygande-korven-logo.png` med en användbar alternativtext.
- Behåll `menu.txt` som oförändrat textunderlag.

CSS-filen är redan kopplad till sidan men är tom från början. Styling kommer under lektion 2.

**Miniminivå idag:** du har själv ändrat filen, sparat, sett resultatet i Chrome och kan hitta tillbaka till projektet.

**Till nästa gång:** färdigställ hela Korvens innehåll med rubriker, stycken, menylista, logotyp, telefonnummer och öppettider. Styling kommer nästa gång.

**När du är klar:** prova att samla sidans delar i `header`, `main` och `footer`, och lägg till en navigationslänk till menyn. Detta är frivillig fördjupning.

## Lektion 2 — spara historik och publicera ditt eget repo

Nu behöver du [GitHub Desktop](https://desktop.github.com/) och ett eget GitHub-konto som du kan logga in på. Vi använder projektmappen från lektion 1, inklusive din egen HTML.

### 4. Förbered GitHub Desktop

1. Öppna GitHub Desktop och logga in på ditt GitHub-konto via webbläsaren.
2. Öppna **GitHub Desktop → Settings** på Mac eller **File → Options** på Windows.
3. Under **Git**, kontrollera ditt namn och välj en e-postadress som hör till ditt konto. Spara.

### 5. Gör den befintliga projektmappen till ett repository

Ett repository, eller repo, är ditt projekt med versionshistorik.

1. Välj **File → Add Local Repository** i GitHub Desktop.
2. Välj exakt samma `flygande-korven`-mapp som du arbetade i under lektion 1.
3. GitHub Desktop säger att mappen inte är ett Git-repository. Klicka på länken **create a repository here**.
4. Behåll det förifyllda namnet och sökvägen. Då används den befintliga mappen.
5. Låt **Initialize this repository with a README** vara avmarkerat; det finns redan en README.
6. Klicka på **Create Repository**.
7. Titta under **History**. GitHub Desktop har skapat en första commit, **Initial commit**, som innehåller dina befintliga filer.
8. Klicka på **Publish repository**. Kontrollera att det är ditt eget konto som står som ägare.
9. För ett publikt kursrepo: avmarkera **Keep this code private**, enligt lärarens instruktion. Klicka sedan på **Publish repository**.
10. Öppna ditt eget repo på GitHub och kontrollera att filerna och din HTML finns där.

Om GitHub Desktop i steg 3 hittar ett befintligt repo: lägg till det och kontrollera historiken tillsammans med läraren. Skapa inte en extra projektmapp.

Publicering av repot gör koden tillgänglig på GitHub. Publicering av själva webbplatsen med GitHub Pages går vi igenom senare.

### 6. Öva på commit och push med en ny ändring

Den första committen finns redan. Gör nu en liten ny ändring för att prova arbetsflödet:

1. Öppna samma projektmapp i VS Code. Du kan använda **Open in Visual Studio Code** i GitHub Desktop.
2. Gör en liten förbättring i `index.html`, till exempel en tydligare rubrik. Spara och kontrollera resultatet i Chrome.
3. Gå till **Changes** i GitHub Desktop. Klicka på `index.html` och granska skillnaden mellan den gamla och den nya versionen.
4. Skriv en beskrivning av ändringen i **Summary**, exempelvis `Förtydligar menyns rubrik`.
5. Klicka på **Commit to main**. Om din lokala gren har ett annat namn visas det namnet på knappen.
6. Klicka på **Push origin** för att skicka committen till GitHub.
7. Kontrollera på GitHub att den nya committen och ändringen finns i ditt eget repo.

Om knappen för VS Code inte visas: välj VS Code som **External editor** under **Integrations** i GitHub Desktops inställningar. Du kan också öppna projektmappen direkt i VS Code.

## Fortsättning — CSS

Under lektion 2 provar vi typografi, färger, mått, padding, margin och border. Fortsätt sedan med styling enligt lärarens uppgift och den visuella referensen.

Efter varje avgränsad förbättring: spara, kontrollera i Chrome, granska ändringen i GitHub Desktop, gör en commit och pusha.

## Klart när

- allt innehåll från `menu.txt` finns på sidan;
- rubriker, listor och sektioner har en begriplig struktur;
- logotypen visas och har alternativtext;
- sidan kan visas lokalt i Chrome;
- du har provat styling enligt lektionens instruktioner;
- projektet finns i ditt eget GitHub-repo;
- du har granskat, committat och pushat minst en ny ändring efter den första publiceringen.
