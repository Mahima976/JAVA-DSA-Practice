// Ternary Operator Syntax: condition ? resultIfTrue : resultIfFalse 
/*
Problem: Cigar Party

A squirrel party is successful when the number of cigars is between 40 and 60 (inclusive),
unless it's the weekend — then there's no upper bound.

Return true if the party is successful.

Examples:
cigarParty(30, false) → false
cigarParty(50, false) → true
cigarParty(70, true)  → true
*/

public class CigarParty {

    // Using if-else
    public boolean cigarPartyIfElse(int cigars, boolean isWeekend) {
        if (isWeekend) {
            return cigars >= 40;
        }
        return cigars >= 40 && cigars <= 60;
    }

    // Using ternary operator
    public boolean cigarPartyTernary(int cigars, boolean isWeekend) {
        return isWeekend ? cigars >= 40 : (cigars >= 40 && cigars <= 60);
    }
}
