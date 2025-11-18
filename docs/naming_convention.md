# Naming convention

I nomi delle classi, metodi e funzioni devono essere parlanti ed esplicativi.
La lingua da utilizzare è l'inglese.

1. Utilizzare la convenzione CamelCase (PascalCase)
2. Tutte le parole riservate colorate dall’IDE Delphi devono essere in minuscolo
   `procedure, string, begin, end ...`
3. La prima lettera delle variabili rispetta la seguente convenzione:
   -   `F` variabili private di classe (fields)
   -   `A` parametri di metodi
   -   `L` variabili locali
4. Le costanti che contengono stringhe o numerici fissi sono tutte in maiuscolo con i nomi separati da under-score (Snake Case)
   `ERP_EXE_NAME` [^1].

   Le **const** locali che non contengono magic word/number seguono la convenzione del punto 3.

[^1]: Sentire FLuzzi per escludere da sonar il controllo sul case della constante.

5. I tipi di dato (classi, record, tipi enumerati etc.) devono iniziare con la lettera `T` maiuscola
   Eccezion fatta per gli attributi.
   
6. Se si decide di utilizzare l'enumerato senza la clausola `{$SCOPEDENUMS ON}` gli elementi devono iniziare con un prefisso minuscolo, costruito con le iniziali delle parole che costituiscono il nome del tipo enumerato.

   `TExpressionComparisonOperator = (ecoEqual, ecoNotEqual, ..)`

8. Lo statement **begin** deve essere sempre posto a capo dello statement precedente 
```delphi
for I := 0 to 10 do begin //  Incorrect, begin on same line as for

for I := 0 to 10 do       //  Correct, begin appears on a separate line
begin
end;
```
9. I nomi delle resourcestring devono rispettare le seguenti regole:
   - iniziare con `RS_`
   - proseguire con contesto di appartenenza
   - terminare con una descrizione sintetica e parlante del contenuto scritta in PascalCase
     
   `RS_WebService_FileNotFound`

11. Evitare nomi criptici o eccessivamente lunghi

| Nome                                                | Approvato |
|-----------------------------------------------------|-----------|
|`CSGetVerAppFromCodInsV2`                            |    ❌    |
|`CSGetVersionApplicationFromInstallationCodeVersion2`|    ❌    |
|`ERPVersionFromInstallationCode`                     |    ✔️    |
