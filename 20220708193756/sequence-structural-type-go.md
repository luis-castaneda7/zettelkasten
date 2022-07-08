# sequence-structural-type-go

in golang two struct types are identical if the have the same sequence
of fields.
ie.
string  ==  string 
int     ==  int

but 
string != int
int    != string
