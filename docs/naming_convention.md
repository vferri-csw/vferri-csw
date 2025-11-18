
I nomi delle classi, metodi e funzioni devono essere parlanti ed esplicativi.
Utilizzare l'inglese per assegnare i nomi di classi, metodi, proprietà, variabili, ecc..

1. Utilizzare la convenzione CamelCase (PascalCase)
2. Tutte le parole riservate colorate dall’IDE Delphi devono essere in minuscolo
   `procedure, string, begin, end ...`

3. Solo le costanti sono tutte in maiuscolo con i nomi separati da under-score (Snake Case)
   `ERP_EXE_NAME`


  * I tipi di dato (classi, record, tipi enumerati etc.) devono iniziare con la lettera **T** maiuscola \\ ''TSimpleClass, TDriveType''

  * Gli elementi dei tipi enumerati dovrebbero iniziare con un prefisso di tre lettere, minuscolo, costruito con le iniziali delle parole che costituiscono il nome del tipo enumerato. \\ ''TExpressionComparisonOperator = (ecoEqual, ecoNotEqual, ..)''

  * Gli oggetti (classi di tipo TOStd) dovrebbero riportare la stringa "Obj" a seguito dell'eventuale prefisso, come da regole precedenti

  * lo statement begin deve essere sempre posto a capo dello statement precedente <code Text [highlight_lines_extra="3,4,5"]>
for I := 0 to 10 do begin //  Incorrect, begin on same line as for

for I := 0 to 10 do       //  Correct, begin appears on a separate line
begin
end;
</code>

  * I parametri in ingresso a un metodo devono iniziare con la lettera **A** maiuscola \\ ''Function SampleProc(AValue: Integer): string;''

  * Le variabili locali a un metodo devono iniziare con la lettera **L** maiuscola \\ <code Delphi [highlight_lines_extra="3"]>
function SampleProc(AValue: Integer): string;
var
  LString: string;  
begin
  LString := 'Example';
  Result := LString +': '+IntToStr(AValue);
end; 
</code> 
