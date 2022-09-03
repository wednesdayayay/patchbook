
[graphviz engine=dot]
digraph structs {node [shape=record];
{

pen:bo -> mem:d

mem:ro -> fkg:fgri
mem:go -> fkg:fggi
mem:bo -> fkg:fgbi

fkg:ro -> vis:ar
fkg:go -> vis:ag
fkg:bo -> vis:ab


vis:comvo -> "main out"


    mem [label="Memory\nPalace |{ 
    { <ri> R | <gi> G | <bi> B | <aux> Aux | <d> Delay | <z> Zoom | <r> Rotation } |
    {<yo> Y | <ro> R | <go> G | <bo> B } }} "];

    vis [label="Visual\nCortex |{ 
    { <ar> A R  | <ag> G | <ab> B }| { <comvo> Component} }  } "];

    pen [label="Pendulum |{ 
    { <ai> A--D | <bi> B--C | <cvc> Crossfade VC }|     
    { <ao> LFO A | <bo> LFO B | <co> C | <do> D } }  } "];

    fkg [label="FKG3|{ 
    { <bgri> BG R | <bggi> G | <bgbi> B | <fgri> FG R | <fggi> G | <fgbi> B | <kri> Key R | <kgi> G | <kbi> B  | <tcv> Thresh | <scv> Soft }|    
    { <ro> R | <go> G | <bo> B} }  } "];


}}
[/graphviz]# patchbook
lzx Graphviz patch book

