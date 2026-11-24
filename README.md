Jeg satte breakpoints i IntelliJ og fulgte spillet fra main til play.
Jeg brugte Evaluate Expression og så, at nextInt(1) altid gav 0.
Jeg rettede det, så skibet kan ligge både vandret og lodret.
I isSunk() så jeg, at hitCount var 3, men at 3 > 3 gav false.
Jeg ændrede > til >=, så skibet synker ved tredje træffer.
Da spillet gik ned, viste debuggeren, at skibets slutpunkt var (10, 4).
Jeg tilføjede isWithinGrid() for at tjekke, om slutpunktet er på brættet.
Hvis skibet går ud over kanten, vælger løkken en ny placering.
